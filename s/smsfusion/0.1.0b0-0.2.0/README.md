# Comparing `tmp/smsfusion-0.1.0b0-py3-none-any.whl.zip` & `tmp/smsfusion-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,19 @@
-Zip file size: 23434 bytes, number of entries: 14
--rw-r--r--  2.0 unx       24 b- defN 20-Feb-02 00:00 smsfusion/__about__.py
--rw-r--r--  2.0 unx      213 b- defN 20-Feb-02 00:00 smsfusion/__init__.py
+Zip file size: 26338 bytes, number of entries: 17
+-rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 smsfusion/__about__.py
+-rw-r--r--  2.0 unx      241 b- defN 20-Feb-02 00:00 smsfusion/__init__.py
 -rw-r--r--  2.0 unx     9220 b- defN 20-Feb-02 00:00 smsfusion/_ahrs.py
--rw-r--r--  2.0 unx    30059 b- defN 20-Feb-02 00:00 smsfusion/_ins.py
+-rw-r--r--  2.0 unx    33165 b- defN 20-Feb-02 00:00 smsfusion/_ins.py
 -rw-r--r--  2.0 unx     9280 b- defN 20-Feb-02 00:00 smsfusion/_transforms.py
 -rw-r--r--  2.0 unx     2226 b- defN 20-Feb-02 00:00 smsfusion/_vectorops.py
 -rw-r--r--  2.0 unx      489 b- defN 20-Feb-02 00:00 smsfusion/benchmark/__init__.py
 -rw-r--r--  2.0 unx    24303 b- defN 20-Feb-02 00:00 smsfusion/benchmark/_benchmark.py
--rw-r--r--  2.0 unx      165 b- defN 20-Feb-02 00:00 smsfusion/noise/__init__.py
+-rw-r--r--  2.0 unx       59 b- defN 20-Feb-02 00:00 smsfusion/calibrate/__init__.py
+-rw-r--r--  2.0 unx     1462 b- defN 20-Feb-02 00:00 smsfusion/calibrate/_calibrate.py
+-rw-r--r--  2.0 unx      235 b- defN 20-Feb-02 00:00 smsfusion/noise/__init__.py
+-rw-r--r--  2.0 unx     2369 b- defN 20-Feb-02 00:00 smsfusion/noise/_allan.py
 -rw-r--r--  2.0 unx    15163 b- defN 20-Feb-02 00:00 smsfusion/noise/_noise.py
-?rw-r--r--  2.0 unx      707 b- defN 20-Feb-02 00:00 smsfusion-0.1.0b0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 smsfusion-0.1.0b0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1064 b- defN 20-Feb-02 00:00 smsfusion-0.1.0b0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1127 b- defN 20-Feb-02 00:00 smsfusion-0.1.0b0.dist-info/RECORD
-14 files, 94127 bytes uncompressed, 21572 bytes compressed:  77.1%
+?rw-r--r--  2.0 unx      705 b- defN 20-Feb-02 00:00 smsfusion-0.2.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 smsfusion-0.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1064 b- defN 20-Feb-02 00:00 smsfusion-0.2.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1377 b- defN 20-Feb-02 00:00 smsfusion-0.2.0.dist-info/RECORD
+17 files, 101467 bytes uncompressed, 24086 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -18,26 +18,35 @@
 
 Filename: smsfusion/benchmark/__init__.py
 Comment: 
 
 Filename: smsfusion/benchmark/_benchmark.py
 Comment: 
 
+Filename: smsfusion/calibrate/__init__.py
+Comment: 
+
+Filename: smsfusion/calibrate/_calibrate.py
+Comment: 
+
 Filename: smsfusion/noise/__init__.py
 Comment: 
 
+Filename: smsfusion/noise/_allan.py
+Comment: 
+
 Filename: smsfusion/noise/_noise.py
 Comment: 
 
-Filename: smsfusion-0.1.0b0.dist-info/METADATA
+Filename: smsfusion-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: smsfusion-0.1.0b0.dist-info/WHEEL
+Filename: smsfusion-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: smsfusion-0.1.0b0.dist-info/licenses/LICENSE
+Filename: smsfusion-0.2.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: smsfusion-0.1.0b0.dist-info/RECORD
+Filename: smsfusion-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## smsfusion/__about__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.0b0"
+__version__ = "0.2.0"
```

## smsfusion/__init__.py

```diff
@@ -1,12 +1,13 @@
-from . import benchmark, noise
+from . import benchmark, calibrate, noise
 from ._ahrs import AHRS
 from ._ins import AidedINS, StrapdownINS, gravity
 
 __all__ = [
     "AHRS",
     "AidedINS",
     "benchmark",
+    "calibrate",
     "gravity",
     "noise",
     "StrapdownINS",
 ]
```

## smsfusion/_ins.py

```diff
@@ -392,103 +392,91 @@
         self._vel = self._vel + self._dt * acc
         self._q_nm = self._q_nm + self._dt * T @ w_ins
         self._q_nm = _normalize(self._q_nm)
 
         return self
 
 
-def _gibbs_scaled(q: NDArray[np.float64]) -> NDArray[np.float64]:
+def _h_head(q: NDArray[np.float64]) -> float:
     """
-    Compute the scaled Gibbs vector (i.e., 2 x Gibbs vector) from a unit quaternion.
+    Compute yaw angle from unit quaternion.
+
+    Defined in terms of scaled Gibbs vector in ref [1]_, but implemented in terms of
+    unit quaternion here to avoid singularities.
 
     Parameters
     ----------
     q : numpy.ndarray, shape (4,)
         Unit quaternion.
 
     Returns
     -------
-    numpy.ndarray, shape (3,)
-        Scaled Gibbs vector.
-    """
-    return (2.0 / q[0]) * q[1:]  # type: ignore[no-any-return]
-
-
-def _h_head(a: NDArray[np.float64]) -> float:
-    """
-    Compute yaw angle from scaled Gibbs vector, see ref [1]_.
-
-    Parameters
-    ----------
-    a : numpy.ndarray, shape (3,)
-        Scaled Gibbs vector.
-
-    Returns
-    -------
     float
         Yaw angle in the NED reference frame.
 
     References
     ----------
     .. [1] Fossen, T.I., "Handbook of Marine Craft Hydrodynamics and Motion Control",
     2nd Edition, equation 14.251, John Wiley & Sons, 2021.
     """
-    a_x, a_y, a_z = a
-    u_y = 2.0 * (a_x * a_y + 2.0 * a_z)
-    u_x = 4.0 + a_x**2 - a_y**2 - a_z**2
+    q_w, q_x, q_y, q_z = q
+    u_y = 2.0 * (q_x * q_y + q_z * q_w)
+    u_x = 1.0 - 2.0 * (q_y**2 + q_z**2)
     return np.arctan2(u_y, u_x)  # type: ignore[no-any-return]
 
 
-def _dhda_head(a: NDArray[np.float64]) -> NDArray[np.float64]:
+def _dhda_head(q: NDArray[np.float64]) -> NDArray[np.float64]:
     """
-    Compute yaw angle gradient wrt to the scaled Gibbs vector, see ref [1]_.
+    Compute yaw angle gradient wrt to the unit quaternion.
+
+    Defined in terms of scaled Gibbs vector in ref [1]_, but implemented in terms of
+    unit quaternion here to avoid singularities.
 
     Parameters
     ----------
-    a : numpy.ndarray, shape (3,)
-        Scaled Gibbs vector.
+    q : numpy.ndarray, shape (3,)
+        Unit quaternion.
 
     Returns
     -------
     numpy.ndarray, shape (3,)
         Yaw angle gradient vector.
 
     References
     ----------
     .. [1] Fossen, T.I., "Handbook of Marine Craft Hydrodynamics and Motion Control",
     2nd Edition, equation 14.254, John Wiley & Sons, 2021.
     """
-    a_x, a_y, a_z = a
-
-    u_y = 2.0 * (a_x * a_y + 2.0 * a_z)
-    u_x = 4.0 + a_x**2 - a_y**2 - a_z**2
+    q_w, q_x, q_y, q_z = q
+    u_y = 2.0 * (q_x * q_y + q_z * q_w)
+    u_x = 1.0 - 2.0 * (q_y**2 + q_z**2)
     u = u_y / u_x
 
-    duda_scale = 1.0 / (4.0 + a_x**2 - a_y**2 - a_z**2) ** 2
-    duda_x = -2.0 * ((a_x**2 + a_z**2 - 4.0) * a_y + a_y**3 + 4.0 * a_x * a_z)
-    duda_y = 2.0 * ((a_y**2 - a_z**2 + 4.0) * a_x + a_x**3 + 4.0 * a_y * a_z)
-    duda_z = 4.0 * (a_z**2 + a_x * a_y * a_z + a_x**2 - a_y**2 + 4.0)
+    duda_scale = 1.0 / u_x**2
+    duda_x = -(q_w * q_y) * (1.0 - 2.0 * q_w**2) - (2.0 * q_w**2 * q_x * q_z)
+    duda_y = (q_w * q_x) * (1.0 - 2.0 * q_z**2) + (2.0 * q_w**2 * q_y * q_z)
+    duda_z = q_w**2 * (1.0 - 2.0 * q_y**2) + (2.0 * q_w * q_x * q_y * q_z)
     duda = duda_scale * np.array([duda_x, duda_y, duda_z])
 
-    dhda = 1.0 / (1.0 + np.sum(u**2)) * duda
+    dhda = 1.0 / (1.0 + u**2) * duda
 
     return dhda  # type: ignore[no-any-return]
 
 
 class AidedINS(INSMixin):
     """
     Aided inertial navigation system (AINS) using a multiplicative extended
     Kalman filter (MEKF).
 
     Parameters
     ----------
     fs : float
         Sampling rate in Hz.
     x0 : array-like, shape (16,)
-        Initial state vector containing the following elements in order:
+        Initial INS state vector containing the following elements in order:
 
         * Position in x, y, z directions (3 elements).
         * Velocity in x, y, z directions (3 elements).
         * Attitude as unit quaternion (4 elements).
         * Accelerometer bias in x, y, z directions (3 elements).
         * Gyroscope bias in x, y, z directions (3 elements).
     P0_prior : array-like, shape (15, 15)
@@ -508,19 +496,31 @@
         * ``tau_cb``: Bias correlation time in seconds.
     var_pos : array-like, shape (3,), optional
         Variance of position measurement noise in m^2.
     var_vel : array-like, shape (3,), optional
         Variance of velocity measurement noise in (m/s)^2.
     var_g : array-like, shape (3,), optional
         Variance of gravitational reference vector measurement noise in m^2.
-    var_compass : float, optional
-        Variance of compass measurement noise in rad^2.
+    var_head : float, optional
+        Variance of heading measurement noise in rad^2.
     lat : float, optional
         Latitude used to calculate the gravitational acceleration. If none
         provided, the 'standard gravity' is assumed.
+    reset_bias_acc : bool, default True
+        Specifies whether to reset the accelerometer bias after each update cycle. If
+        set to ``True``, the estimated error-state bias is incorporated into the
+        strapdown algorithm's bias state, effectively resetting the error-state bias to
+        zero. Defaults to ``True``.
+    reset_bias_gyro : bool, default True
+        Specifies whether to reset the gyroscope bias after each update cycle. If set to
+        ``True``, the estimated error-state bias is incorporated into the strapdown
+        algorithm's bias state, effectively resetting the error-state bias to zero.
+        Defaults to ``True``.
+    dx0_prior : array-like, shape (15,), default numpy.zeros(15)
+        Initial a priori estimate of the error-state vector. Defaults to ``numpy.zeros(15)``.
     """
 
     _I15 = np.eye(15)
 
     def __init__(
         self,
         fs: float,
@@ -529,25 +529,25 @@
         err_acc: dict[str, float],
         err_gyro: dict[str, float],
         var_pos: ArrayLike | None = None,
         var_vel: ArrayLike | None = None,
         var_g: ArrayLike | None = None,
         var_head: float | None = None,
         lat: float | None = None,
+        reset_bias_acc: bool = True,
+        reset_bias_gyro: bool = True,
+        dx0_prior: ArrayLike = np.zeros(15),
     ) -> None:
         self._fs = fs
         self._dt = 1.0 / fs
-        self._x0 = np.asarray_chkfinite(x0).reshape(16).copy()
-        self._x0[6:10] = _normalize(self._x0[6:10])
-        self._x = self._x0.copy()
-        self._P0_prior = np.asarray_chkfinite(P0_prior).reshape(15, 15).copy()
-        self._P_prior = self._P0_prior.copy()
-        self._P = np.empty_like(self._P_prior)
         self._err_acc = err_acc
         self._err_gyro = err_gyro
+        self._lat = lat
+        self._reset_bias_acc = reset_bias_acc
+        self._reset_bias_gyro = reset_bias_gyro
 
         if var_pos is not None:
             var_pos = np.asarray_chkfinite(var_pos).reshape(3).copy()
         if var_vel is not None:
             var_vel = np.asarray_chkfinite(var_vel).reshape(3).copy()
         if var_g is not None:
             var_g = np.asarray_chkfinite(var_g).reshape(3).copy()
@@ -555,24 +555,79 @@
             var_head = np.asarray_chkfinite(var_head).reshape(1).copy()
 
         self._var_pos = var_pos
         self._var_vel = var_vel
         self._var_g = var_g
         self._var_head = var_head
 
+        # Error-state
+        self._dx = np.zeros(15)
+
         # Strapdown algorithm
-        self._ins = StrapdownINS(self._fs, self._x0, lat=lat)
+        self._ins = StrapdownINS(self._fs, x0, lat=self._lat)
+
+        # Total state
+        self._x = self._combine_states(self._ins._x, self._dx)
+
+        # Initialize Kalman filter
+        self._dx_prior = np.asarray_chkfinite(dx0_prior).reshape(15).copy()
+        self._P_prior = np.asarray_chkfinite(P0_prior).reshape(15, 15).copy()
+        self._P = np.empty_like(self._P_prior)
 
         # Prepare system matrices
-        q0 = self._x0[6:10]
+        q0 = self._ins._q_nm
         self._F = self._prep_F(err_acc, err_gyro, q0)
         self._G = self._prep_G(q0)
         self._H = self._prep_H(q0)
         self._W = self._prep_W(err_acc, err_gyro)
 
+    def dump(self):
+        """
+        Dump the configuration and current state of the AINS to a dictionary. The dumped
+        parameters can be used to restore the AINS to its current state.
+
+        Returns
+        -------
+        dict
+            A dictionary containing the configuration and current state of the AINS.
+        """
+        params = {
+            "fs": self._fs,
+            "x0": self._ins._x.tolist(),
+            "P0_prior": self._P_prior.tolist(),
+            "err_acc": self._err_acc,
+            "err_gyro": self._err_gyro,
+            "var_pos": self._var_pos.tolist() if self._var_pos is not None else None,
+            "var_vel": self._var_vel.tolist() if self._var_vel is not None else None,
+            "var_g": self._var_g.tolist() if self._var_g is not None else None,
+            "var_head": self._var_head.tolist() if self._var_head is not None else None,
+            "lat": self._lat,
+            "reset_bias_acc": self._reset_bias_acc,
+            "reset_bias_gyro": self._reset_bias_gyro,
+            "dx0_prior": self._dx_prior.tolist(),
+        }
+        return params
+
+    @staticmethod
+    def _combine_states(x_ins, dx):
+        """
+        Combine the INS state with the error-state estimate to form the total state
+        estimate.
+        """
+        da = dx[6:9]
+        dq = (1.0 / np.sqrt(4.0 + da.T @ da)) * np.r_[2.0, da]
+        pos = x_ins[0:3] + dx[0:3]
+        vel = x_ins[3:6] + dx[3:6]
+        q_nm = _quaternion_product(x_ins[6:10], dq)
+        q_nm = _normalize(q_nm)
+        bias_acc = x_ins[10:13] + dx[9:12]
+        bias_gyro = x_ins[13:16] + dx[12:15]
+        x = np.r_[pos, vel, q_nm, bias_acc, bias_gyro]
+        return x
+
     @property
     def P(self) -> NDArray[np.float64]:
         """
         Current updated error covariance matrix, **P**. I.e., the error covariance
         matrix associated with the Kalman filter's updated (a posteriori) error-state
         estimate.
         """
@@ -664,28 +719,28 @@
         S = _skew_symmetric  # alias skew symmetric matrix
         R_nm = _rot_matrix_from_quaternion(q_nm)  # body-to-ned rotation matrix
 
         H = np.zeros((10, 15))
         H[0:3, 0:3] = np.eye(3)  # position
         H[3:6, 3:6] = np.eye(3)  # velocity
         H[6:9, 6:9] = S(R_nm.T @ vg_ref_n)  # gravity reference vector
-        H[9:10, 6:9] = _dhda_head(_gibbs_scaled(q_nm))  # compass
+        H[9:10, 6:9] = _dhda_head(q_nm)  # compass
         return H
 
     def _update_H(self, q_nm: NDArray[np.float64]) -> None:
         """Update linearized measurement matrix, H."""
 
         # Reference vector
         vg_ref_n = np.array([0.0, 0.0, 1.0])
 
         S = _skew_symmetric  # alias skew symmetric matrix
         R_nm = _rot_matrix_from_quaternion(q_nm)  # body-to-ned rotation matrix
 
         self._H[6:9, 6:9] = S(R_nm.T @ vg_ref_n)  # gravity reference vector
-        self._H[9:10, 6:9] = _dhda_head(_gibbs_scaled(q_nm))  # compass
+        self._H[9:10, 6:9] = _dhda_head(q_nm)  # compass
 
     @staticmethod
     def _prep_W(
         err_acc: dict[str, float], err_gyro: dict[str, float]
     ) -> NDArray[np.float64]:
         """Prepare white noise power spectral density matrix"""
         N_acc = err_acc["N"]
@@ -699,21 +754,38 @@
         W = np.eye(12)
         W[0:3, 0:3] *= N_acc**2
         W[3:6, 3:6] *= N_gyro**2
         W[6:9, 6:9] *= 2.0 * sigma_acc**2 * beta_acc
         W[9:12, 9:12] *= 2.0 * sigma_gyro**2 * beta_gyro
         return W
 
+    def _reset(self) -> None:
+        """Reset"""
+        x_ins = np.r_[
+            self._x[:10],
+            self._x[10:13] if self._reset_bias_acc else self._ins._bias_acc,
+            self._x[13:16] if self._reset_bias_gyro else self._ins._bias_gyro,
+        ]
+        self._ins.reset(x_ins)
+
+        dx = np.r_[
+            np.zeros(9),
+            np.zeros(3) if self._reset_bias_acc else self._dx[9:12],
+            np.zeros(3) if self._reset_bias_gyro else self._dx[12:15],
+        ]
+        self._dx = dx
+
     def update(
         self,
         f_imu: ArrayLike,
         w_imu: ArrayLike,
         pos: ArrayLike | None = None,
         vel: ArrayLike | None = None,
         head: float | None = None,
+        g_ref: bool = False,
         degrees: bool = False,
         head_degrees: bool = True,
         var_pos: ArrayLike | None = None,
         var_vel: ArrayLike | None = None,
         var_g: ArrayLike | None = None,
         var_head: float | None = None,
     ) -> "AidedINS":  # TODO: Replace with ``typing.Self`` when Python > 3.11
@@ -732,14 +804,16 @@
             and z-axis, respectively.
         pos : array-like, shape (3,), optional
             Position aiding measurement. If ``None``, position aiding is not used.
         vel : array-like, shape (3,), optional
             Velocity aiding measurement. If ``None``, velocity aiding is not used.
         head : float, optional
             Heading measurement, i.e., yaw angle. If ``None``, compass aiding is not used.
+        g_ref : bool, optional, default False
+            Specifies whether the gravity reference vector is used as an aiding measurement.
         degrees : bool, default False
             Specifies whether the unit of ``w_imu`` are in degrees or radians.
         head_degrees : bool, default True
             Specifies whether the unit of ``head`` are in degrees or radians.
         var_pos : array-like, shape (3,), optional
             Variance of position measurement noise in m^2.
         var_vel : array-like, shape (3,), optional
@@ -756,23 +830,20 @@
         """
         f_imu = np.asarray_chkfinite(f_imu, dtype=float).reshape(3).copy()
         w_imu = np.asarray_chkfinite(w_imu, dtype=float).reshape(3).copy()
 
         if degrees:
             w_imu = (np.pi / 180.0) * w_imu
 
-        # Update current state estimate
-        self._x = self._ins.x
-
-        # Current state estimates
-        pos_ins = self._pos
-        vel_ins = self._vel
-        q_ins_nm = self._q_nm
-        bias_acc_ins = self._bias_acc
-        bias_gyro_ins = self._bias_gyro
+        # Current INS state estimates
+        pos_ins = self._ins._pos
+        vel_ins = self._ins._vel
+        q_ins_nm = self._ins._q_nm
+        bias_acc_ins = self._ins._bias_acc
+        bias_gyro_ins = self._ins._bias_gyro
 
         R_ins_nm = _rot_matrix_from_quaternion(q_ins_nm)  # body-to-ned rotation matrix
 
         # Bias compensated IMU measurements
         f_ins = f_imu - bias_acc_ins
         w_ins = w_imu - bias_gyro_ins
 
@@ -811,79 +882,75 @@
                 raise ValueError("'var_vel' not provided.")
 
             dz_temp.append(delta_vel)
             var_z_temp.append(var_vel)
             H_temp.append(self._H[3:6])
 
         # Gravity reference vector aiding
-        vg_ref_n = np.array([0.0, 0.0, 1.0])
-        vg_meas_m = -_normalize(f_ins)
-        delta_g = vg_meas_m - R_ins_nm.T @ vg_ref_n
+        if g_ref:
+            vg_ref_n = np.array([0.0, 0.0, 1.0])
+            vg_meas_m = -_normalize(f_imu - self._bias_acc)
+            delta_g = vg_meas_m - R_ins_nm.T @ vg_ref_n
+
+            if var_g is not None:
+                var_g = np.asarray_chkfinite(var_g, dtype=float).reshape(3).copy()
+            elif self._var_g is not None:
+                var_g = self._var_g
+            else:
+                raise ValueError("'var_g' not provided.")
 
-        if var_g is not None:
-            var_g = np.asarray_chkfinite(var_g, dtype=float).reshape(3).copy()
-        elif self._var_g is not None:
-            var_g = self._var_g
-        else:
-            raise ValueError("'var_g' not provided.")
-
-        dz_temp.append(delta_g)
-        var_z_temp.append(var_g)
-        H_temp.append(self._H[6:9])
+            dz_temp.append(delta_g)
+            var_z_temp.append(var_g)
+            H_temp.append(self._H[6:9])
 
         # Compass aiding
         if head is not None:
             if head_degrees:
                 head = (np.pi / 180.0) * head
-            delta_head = _signed_smallest_angle(
-                head - _h_head(_gibbs_scaled(q_ins_nm)), degrees=False
-            )
+            delta_head = _signed_smallest_angle(head - _h_head(q_ins_nm), degrees=False)
 
             if var_head is not None:
                 var_head = np.asarray_chkfinite(var_head, dtype=float).reshape(1).copy()
             elif self._var_head is not None:
                 var_head = self._var_head
             else:
                 raise ValueError("'var_head' not provided.")
 
             dz_temp.append(np.array([delta_head]))
             var_z_temp.append(var_head)
             H_temp.append(self._H[-1:])
 
-        dz = np.concatenate(dz_temp, axis=0)
-        H = np.concatenate(H_temp, axis=0)
-        R = np.diag(np.concatenate(var_z_temp, axis=0))
+        if dz_temp:
+            dz = np.concatenate(dz_temp, axis=0)
+            H = np.concatenate(H_temp, axis=0)
+            R = np.diag(np.concatenate(var_z_temp, axis=0))
+
+            # Compute Kalman gain
+            K = self._P_prior @ H.T @ inv(H @ self._P_prior @ H.T + R)
+
+            # Update error-state estimate with measurement
+            self._dx = self._dx_prior + K @ dz
+
+            # Compute error covariance for updated estimate
+            self._P = (self._I15 - K @ H) @ self._P_prior @ (
+                self._I15 - K @ H
+            ).T + K @ R @ K.T
+        else:  # no aiding measurements
+            self._P = self._P_prior
+            self._dx = self._dx_prior
 
         # Discretize system
         phi = self._I15 + self._dt * self._F  # state transition matrix
         Q = self._dt * self._G @ self._W @ self._G.T  # process noise covariance matrix
 
-        # Compute Kalman gain
-        K = self._P_prior @ H.T @ inv(H @ self._P_prior @ H.T + R)
-
-        # Update error-state estimate with measurement
-        dx = K @ dz
-
-        # Compute error covariance for updated estimate
-        self._P = (self._I15 - K @ H) @ self._P_prior @ (
-            self._I15 - K @ H
-        ).T + K @ R @ K.T
-
-        # Error quaternion from 2x Gibbs vector
-        da = dx[6:9]
-        dq = (1.0 / np.sqrt(4.0 + da.T @ da)) * np.r_[2.0, da]
+        # Update (total) state estimate
+        self._x = self._combine_states(self._ins.x, self._dx)
 
         # Reset
-        pos_ins = pos_ins + dx[0:3]
-        vel_ins = vel_ins + dx[3:6]
-        q_ins_nm = _quaternion_product(q_ins_nm, dq)
-        q_ins_nm = _normalize(q_ins_nm)
-        bias_acc_ins = bias_acc_ins + dx[9:12]
-        bias_gyro_ins = bias_gyro_ins + dx[12:15]
-        x_ins = np.r_[pos_ins, vel_ins, q_ins_nm, bias_acc_ins, bias_gyro_ins]
-        self._ins.reset(x_ins)
+        self._reset()
 
         # Project ahead
         self._ins.update(f_imu, w_imu, degrees=False)
+        self._dx_prior = phi @ self._dx
         self._P_prior = phi @ self._P @ phi.T + Q
 
         return self
```

## smsfusion/noise/__init__.py

```diff
@@ -1,3 +1,11 @@
+from ._allan import allan_var
 from ._noise import IMUNoise, NoiseModel, gauss_markov, random_walk, white_noise
 
-__all__ = ["IMUNoise", "NoiseModel", "gauss_markov", "random_walk", "white_noise"]
+__all__ = [
+    "IMUNoise",
+    "NoiseModel",
+    "allan_var",
+    "gauss_markov",
+    "random_walk",
+    "white_noise",
+]
```

## Comparing `smsfusion-0.1.0b0.dist-info/METADATA` & `smsfusion-0.2.0.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: smsfusion
-Version: 0.1.0b0
+Version: 0.2.0
 Summary: Sensor fusion algorithms and utilities for SMS Motion
 Project-URL: Homepage, https://github.com/4Subsea/smsfusion-python
 Project-URL: Bug Tracker, https://github.com/4Subsea/smsfusion-python/issues
 Author-email: 4Subsea <python@4subsea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `smsfusion-0.1.0b0.dist-info/licenses/LICENSE` & `smsfusion-0.2.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

