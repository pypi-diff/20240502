# Comparing `tmp/squishyplanet-0.0.1.tar.gz` & `tmp/squishyplanet-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squishyplanet-0.0.1.tar", last modified: Thu Apr 25 15:47:59 2024, max compression
+gzip compressed data, was "squishyplanet-0.1.0.tar", last modified: Thu May  2 20:41:19 2024, max compression
```

## Comparing `squishyplanet-0.0.1.tar` & `squishyplanet-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-04-25 15:47:59.703447 squishyplanet-0.0.1/
--rw-r--r--   0 cassese    (501) staff       (20)     1068 2024-03-11 14:22:30.000000 squishyplanet-0.0.1/LICENSE
--rw-r--r--   0 cassese    (501) staff       (20)     1339 2024-04-25 15:47:59.703181 squishyplanet-0.0.1/PKG-INFO
--rw-r--r--   0 cassese    (501) staff       (20)      518 2024-04-19 16:09:03.000000 squishyplanet-0.0.1/README.md
--rw-r--r--   0 cassese    (501) staff       (20)     1000 2024-04-25 15:47:03.000000 squishyplanet-0.0.1/pyproject.toml
--rw-r--r--   0 cassese    (501) staff       (20)       38 2024-04-25 15:47:59.703493 squishyplanet-0.0.1/setup.cfg
--rw-r--r--   0 cassese    (501) staff       (20)       90 2024-04-20 21:39:16.000000 squishyplanet-0.0.1/setup.py
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-04-25 15:47:59.699389 squishyplanet-0.0.1/squishyplanet/
--rw-r--r--   0 cassese    (501) staff       (20)      233 2024-04-24 13:17:25.000000 squishyplanet-0.0.1/squishyplanet/__init__.py
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-04-25 15:47:59.701720 squishyplanet-0.0.1/squishyplanet/engine/
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-04-25 15:47:59.702450 squishyplanet-0.0.1/squishyplanet/engine/development/
--rw-r--r--   0 cassese    (501) staff       (20)     4637 2024-04-20 21:39:16.000000 squishyplanet-0.0.1/squishyplanet/engine/development/lambertian_reflectance.py
--rw-r--r--   0 cassese    (501) staff       (20)     9098 2024-04-20 21:39:16.000000 squishyplanet-0.0.1/squishyplanet/engine/development/quadratic_limb_darkened_transit.py
--rw-r--r--   0 cassese    (501) staff       (20)    44246 2024-04-20 21:39:16.000000 squishyplanet-0.0.1/squishyplanet/engine/development/terminator.py
--rw-r--r--   0 cassese    (501) staff       (20)     4383 2024-04-24 17:49:36.000000 squishyplanet-0.0.1/squishyplanet/engine/development/test_emission_normalization.py
--rw-r--r--   0 cassese    (501) staff       (20)     3273 2024-04-20 21:39:16.000000 squishyplanet-0.0.1/squishyplanet/engine/greens_basis_transform.py
--rw-r--r--   0 cassese    (501) staff       (20)     5153 2024-04-20 21:39:16.000000 squishyplanet-0.0.1/squishyplanet/engine/kepler.py
--rw-r--r--   0 cassese    (501) staff       (20)     5478 2024-04-20 21:39:16.000000 squishyplanet-0.0.1/squishyplanet/engine/parametric_ellipse.py
--rw-r--r--   0 cassese    (501) staff       (20)    52332 2024-04-24 18:44:20.000000 squishyplanet-0.0.1/squishyplanet/engine/phase_curve_utils.py
--rw-r--r--   0 cassese    (501) staff       (20)     3482 2024-04-20 21:39:16.000000 squishyplanet-0.0.1/squishyplanet/engine/planet_2d.py
--rw-r--r--   0 cassese    (501) staff       (20)    20153 2024-04-20 21:39:16.000000 squishyplanet-0.0.1/squishyplanet/engine/planet_3d.py
--rw-r--r--   0 cassese    (501) staff       (20)    23936 2024-04-24 21:15:56.000000 squishyplanet-0.0.1/squishyplanet/engine/polynomial_limb_darkened_transit.py
--rw-r--r--   0 cassese    (501) staff       (20)    40307 2024-04-24 21:13:12.000000 squishyplanet-0.0.1/squishyplanet/oblate_system.py
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-04-25 15:47:59.702910 squishyplanet-0.0.1/squishyplanet.egg-info/
--rw-r--r--   0 cassese    (501) staff       (20)     1339 2024-04-25 15:47:59.000000 squishyplanet-0.0.1/squishyplanet.egg-info/PKG-INFO
--rw-r--r--   0 cassese    (501) staff       (20)      877 2024-04-25 15:47:59.000000 squishyplanet-0.0.1/squishyplanet.egg-info/SOURCES.txt
--rw-r--r--   0 cassese    (501) staff       (20)        1 2024-04-25 15:47:59.000000 squishyplanet-0.0.1/squishyplanet.egg-info/dependency_links.txt
--rw-r--r--   0 cassese    (501) staff       (20)       75 2024-04-25 15:47:59.000000 squishyplanet-0.0.1/squishyplanet.egg-info/requires.txt
--rw-r--r--   0 cassese    (501) staff       (20)       14 2024-04-25 15:47:59.000000 squishyplanet-0.0.1/squishyplanet.egg-info/top_level.txt
-drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-04-25 15:47:59.702724 squishyplanet-0.0.1/tests/
--rw-r--r--   0 cassese    (501) staff       (20)     3962 2024-04-24 21:24:42.000000 squishyplanet-0.0.1/tests/test_against_jaxoplanet_transit.py
--rw-r--r--   0 cassese    (501) staff       (20)     3560 2024-04-24 18:44:20.000000 squishyplanet-0.0.1/tests/test_oblate_system.py
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-02 20:41:19.539962 squishyplanet-0.1.0/
+-rw-r--r--   0 cassese    (501) staff       (20)     1068 2024-03-11 14:22:30.000000 squishyplanet-0.1.0/LICENSE
+-rw-r--r--   0 cassese    (501) staff       (20)     2561 2024-05-02 20:41:19.539723 squishyplanet-0.1.0/PKG-INFO
+-rw-r--r--   0 cassese    (501) staff       (20)     1740 2024-05-02 05:57:27.000000 squishyplanet-0.1.0/README.md
+-rw-r--r--   0 cassese    (501) staff       (20)     1000 2024-05-02 20:39:35.000000 squishyplanet-0.1.0/pyproject.toml
+-rw-r--r--   0 cassese    (501) staff       (20)       38 2024-05-02 20:41:19.540005 squishyplanet-0.1.0/setup.cfg
+-rw-r--r--   0 cassese    (501) staff       (20)       90 2024-04-20 21:39:16.000000 squishyplanet-0.1.0/setup.py
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-02 20:41:19.534128 squishyplanet-0.1.0/squishyplanet/
+-rw-r--r--   0 cassese    (501) staff       (20)      233 2024-04-24 13:17:25.000000 squishyplanet-0.1.0/squishyplanet/__init__.py
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-02 20:41:19.537050 squishyplanet-0.1.0/squishyplanet/engine/
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-02 20:41:19.538594 squishyplanet-0.1.0/squishyplanet/engine/development/
+-rw-r--r--   0 cassese    (501) staff       (20)     4637 2024-04-20 21:39:16.000000 squishyplanet-0.1.0/squishyplanet/engine/development/lambertian_reflectance.py
+-rw-r--r--   0 cassese    (501) staff       (20)     9098 2024-04-20 21:39:16.000000 squishyplanet-0.1.0/squishyplanet/engine/development/quadratic_limb_darkened_transit.py
+-rw-r--r--   0 cassese    (501) staff       (20)    44246 2024-04-20 21:39:16.000000 squishyplanet-0.1.0/squishyplanet/engine/development/terminator.py
+-rw-r--r--   0 cassese    (501) staff       (20)     4383 2024-04-24 17:49:36.000000 squishyplanet-0.1.0/squishyplanet/engine/development/test_emission_normalization.py
+-rw-r--r--   0 cassese    (501) staff       (20)     3273 2024-04-20 21:39:16.000000 squishyplanet-0.1.0/squishyplanet/engine/greens_basis_transform.py
+-rw-r--r--   0 cassese    (501) staff       (20)     5153 2024-04-20 21:39:16.000000 squishyplanet-0.1.0/squishyplanet/engine/kepler.py
+-rw-r--r--   0 cassese    (501) staff       (20)     6370 2024-04-26 22:30:04.000000 squishyplanet-0.1.0/squishyplanet/engine/parametric_ellipse.py
+-rw-r--r--   0 cassese    (501) staff       (20)    55107 2024-05-02 20:35:36.000000 squishyplanet-0.1.0/squishyplanet/engine/phase_curve_utils.py
+-rw-r--r--   0 cassese    (501) staff       (20)     3482 2024-04-20 21:39:16.000000 squishyplanet-0.1.0/squishyplanet/engine/planet_2d.py
+-rw-r--r--   0 cassese    (501) staff       (20)    24701 2024-04-30 20:17:55.000000 squishyplanet-0.1.0/squishyplanet/engine/planet_3d.py
+-rw-r--r--   0 cassese    (501) staff       (20)    24137 2024-04-26 21:48:50.000000 squishyplanet-0.1.0/squishyplanet/engine/polynomial_limb_darkened_transit.py
+-rw-r--r--   0 cassese    (501) staff       (20)    51441 2024-05-02 20:35:36.000000 squishyplanet-0.1.0/squishyplanet/oblate_system.py
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-02 20:41:19.539497 squishyplanet-0.1.0/squishyplanet.egg-info/
+-rw-r--r--   0 cassese    (501) staff       (20)     2561 2024-05-02 20:41:19.000000 squishyplanet-0.1.0/squishyplanet.egg-info/PKG-INFO
+-rw-r--r--   0 cassese    (501) staff       (20)      877 2024-05-02 20:41:19.000000 squishyplanet-0.1.0/squishyplanet.egg-info/SOURCES.txt
+-rw-r--r--   0 cassese    (501) staff       (20)        1 2024-05-02 20:41:19.000000 squishyplanet-0.1.0/squishyplanet.egg-info/dependency_links.txt
+-rw-r--r--   0 cassese    (501) staff       (20)       75 2024-05-02 20:41:19.000000 squishyplanet-0.1.0/squishyplanet.egg-info/requires.txt
+-rw-r--r--   0 cassese    (501) staff       (20)       14 2024-05-02 20:41:19.000000 squishyplanet-0.1.0/squishyplanet.egg-info/top_level.txt
+drwxr-xr-x   0 cassese    (501) staff       (20)        0 2024-05-02 20:41:19.539170 squishyplanet-0.1.0/tests/
+-rw-r--r--   0 cassese    (501) staff       (20)     3962 2024-04-24 21:24:42.000000 squishyplanet-0.1.0/tests/test_against_jaxoplanet_transit.py
+-rw-r--r--   0 cassese    (501) staff       (20)     3787 2024-05-01 21:32:33.000000 squishyplanet-0.1.0/tests/test_oblate_system.py
```

### Comparing `squishyplanet-0.0.1/LICENSE` & `squishyplanet-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.0.1/pyproject.toml` & `squishyplanet-0.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "squishyplanet"
-version = "0.0.1"
+version = "0.1.0"
 requires-python = ">=3.9"
 dependencies = [
     "requests",
     "jax",
     "jaxlib",
     "quadax",
     "tqdm",
```

### Comparing `squishyplanet-0.0.1/squishyplanet/engine/development/lambertian_reflectance.py` & `squishyplanet-0.1.0/squishyplanet/engine/development/lambertian_reflectance.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.0.1/squishyplanet/engine/development/quadratic_limb_darkened_transit.py` & `squishyplanet-0.1.0/squishyplanet/engine/development/quadratic_limb_darkened_transit.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.0.1/squishyplanet/engine/development/terminator.py` & `squishyplanet-0.1.0/squishyplanet/engine/development/terminator.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.0.1/squishyplanet/engine/development/test_emission_normalization.py` & `squishyplanet-0.1.0/squishyplanet/engine/development/test_emission_normalization.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.0.1/squishyplanet/engine/greens_basis_transform.py` & `squishyplanet-0.1.0/squishyplanet/engine/greens_basis_transform.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.0.1/squishyplanet/engine/kepler.py` & `squishyplanet-0.1.0/squishyplanet/engine/kepler.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.0.1/squishyplanet/engine/parametric_ellipse.py` & `squishyplanet-0.1.0/squishyplanet/engine/parametric_ellipse.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,35 @@
 
 
 # running into some numerical issues for very narrow ellipses-
 # e.g., the terminator for a spherical planet at f=1e-6. the rhos are ~1e14 there,
 # and the final value for c_y1 is off. everything is fine at f=1e-5 though, so leaving
 # for now
 @jax.jit
-def _poly_to_parametric_helper(
-    rho_xx, rho_xy, rho_x0, rho_yy, rho_y0, rho_00, **kwargs
-):
+def poly_to_parametric_helper(rho_xx, rho_xy, rho_x0, rho_yy, rho_y0, rho_00, **kwargs):
+    """
+    A helper function for :func:`poly_to_parametric`.
+
+    Args:
+        rho_xx (Array [Dimensionless]): Coefficient of x^2
+        rho_xy (Array [Dimensionless]): Coefficient of xy
+        rho_x0 (Array [Dimensionless]): Coefficient of x
+        rho_yy (Array [Dimensionless]): Coefficient of y^2
+        rho_y0 (Array [Dimensionless]): Coefficient of y
+        rho_00 (Array [Dimensionless]): Constant term
+
+    Returns:
+        Tuple:
+            - r1 (Array [Rstar]): Semi-major axis of the projected ellipse
+            - r2 (Array [Rstar]): Semi-minor axis of the projected ellipse
+            - xc (Array [Rstar]): x-coordinate of the center of the ellipse
+            - yc (Array [Rstar]): y-coordinate of the center of the ellipse
+            - cosa (Array [Dimensionless]): Cosine of the rotation angle
+            - sina (Array [Dimensionless]): Sine of the rotation angle
+    """
     rho_00 -= 1
 
     # the center of the ellipse
     xc = (rho_xy * rho_y0 - 2 * rho_yy * rho_x0) / (4 * rho_xx * rho_yy - rho_xy**2)
     yc = (rho_xy * rho_x0 - 2 * rho_xx * rho_y0) / (4 * rho_xx * rho_yy - rho_xy**2)
 
     # the rotation angle
@@ -72,15 +90,15 @@
             Dictionary of coefficients for the parametric ellipse. The ellipse can now
             be described by the following parametric equations for parameter :math:`\\alpha`:
 
             .. math::
                 x = c_{x1} * \\cos(\\alpha) + c_{x2} * \\sin(\\alpha) + c_{x3}
                 y = c_{y1} * \\cos(\\alpha) + c_{y2} * \\sin(\\alpha) + c_{y3}
     """
-    r1, r2, xc, yc, cosa, sina = _poly_to_parametric_helper(
+    r1, r2, xc, yc, cosa, sina = poly_to_parametric_helper(
         rho_xx, rho_xy, rho_x0, rho_yy, rho_y0, rho_00
     )
 
     return {
         "c_x1": r1 * cosa,
         "c_x2": -r2 * sina,
         "c_x3": xc,
```

### Comparing `squishyplanet-0.0.1/squishyplanet/engine/phase_curve_utils.py` & `squishyplanet-0.1.0/squishyplanet/engine/phase_curve_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import jax
 
 jax.config.update("jax_enable_x64", True)
 import jax.numpy as jnp
 
-from squishyplanet.engine.parametric_ellipse import _poly_to_parametric_helper
+from squishyplanet.engine.parametric_ellipse import poly_to_parametric_helper
 from squishyplanet.engine.planet_2d import planet_2d_coeffs
 
 ########################################################################################
 # General helpers
 ########################################################################################
 
 
@@ -51,15 +51,15 @@
     rho_x0,
     rho_yy,
     rho_y0,
     rho_00,
     **kwargs,
 ):
     # n = n.shape[0]
-    r1, r2, xc, yc, cosa, sina = _poly_to_parametric_helper(
+    r1, r2, xc, yc, cosa, sina = poly_to_parametric_helper(
         rho_xx, rho_xy, rho_x0, rho_yy, rho_y0, rho_00
     )
 
     x = r1 * sample_radii * jnp.cos(sample_thetas)
     y = r2 * sample_radii * jnp.sin(sample_thetas)
 
     x_rotated = cosa * x - sina * y
@@ -586,42 +586,58 @@
     the cosine of the angle between the surface normal and the illumination direction.
     That arrangement means it does *not* depend on the observer's viewing angle, only
     the illumination angle. This helper function also assumes a uniform albedo of 1
     across the planet's surface (the final reflected flux will be scaled by the provided
     albedo, though is still always assumed to be uniform).
 
     This function will also mask out any points on the planet's surface that are on the
-    wrong side of the terminator or blocked by the star during secondary eclipse.
+    wrong side of the terminator.
 
     Args:
         surface_star_cos_angle (Array): The cosine of the angle between the planet's
             surface normal and the vector pointing from the planet's center to the star.
         x (Array): The x values of the points on the planet's surface.
         y (Array): The y values of the points on the planet's surface.
         z (Array): The z values of the points on the planet's surface.
 
     Returns:
         Array: The intensity of the reflected light at each point.
 
     """
     # return jnp.maximum(0, surface_star_angle)
-    return (
-        surface_star_cos_angle
-        * (surface_star_cos_angle > 0)
-        * ~((x**2 + y**2 < 1) & (z < 0))
-    )
+    return surface_star_cos_angle * (surface_star_cos_angle > 0)
+
+
+@jax.jit
+def _henyey_greenstein(g, theta):
+    return 0.5 * (1 - g1**2) / (1 + g1**2 - 2 * g * jnp.cos(theta)) ** (1.5)
+
+
+@jax.jit
+def _two_term_henyey_greenstein(gf, gb, scatter_f, theta):
+    return scatter_f * _henyey_greenstein(gf, theta) + (
+        1 - scatter_f
+    ) * _henyey_greenstein(gb, theta)
+
+
+@jax.jit
+def _rayleigh_scattering(theta):
+    return (3 / 4) * (1 + jnp.cos(theta) ** 2)
 
 
 @jax.jit
 def reflected_normalization(
     two,
     three,
     x_c,
     y_c,
     z_c,
+    xo=0.0,
+    yo=0.0,
+    zo=0.0,
     **kwargs,
 ):
     """
     Compute the time-dependent normalization factor for the reflected light.
 
     The reflected light computations are almost entirely carried out assuming the star
     is a point source 1 R_star from the center of the planet emitting plane-parallel
@@ -641,23 +657,36 @@
             :func:`planet_2d.planet_2d_coeffs`.
         three (dict):
             A dictionary containing the p coefficients of the planet's 3D shape, as seen
             from the observer and calculated with :func:`planet_3d.planet_3d_coeffs`.
         x_c (Array): The x coordinate of the center of the planet.
         y_c (Array): The y coordinate of the center of the planet.
         z_c (Array): The z coordinate of the center of the planet.
+        xo (float or Array):
+            An offset to add to the x coordinate of the center of the planet, used when
+            correcting for extended source illuminations. Default is 0.0.
+        yo (float or Array):
+            An offset to add to the y coordinate of the center of the planet, used when
+            correcting for extended source illuminations. Default is 0.0.
+        zo (float or Array):
+            An offset to add to the z coordinate of the center of the planet, used when
+            correcting for extended source illuminations. Default is 0.0.
         **kwargs:
             Additional unused keyword arguments, included so that we can pass in
             a larger state dictionary that includes all of the required parameters along
             with other unnecessary ones.
 
     Returns:
         Array: The normalization factor for the reflected light.
 
     """
+    x_c = x_c - xo
+    y_c = y_c - yo
+    z_c = z_c - zo
+
     sep_squared = x_c**2 + y_c**2 + z_c**2
     # flux_density = 1 / (4 * jnp.pi * sep_squared)
     # following the starry normalization:
     flux_density = 1 / (jnp.pi * sep_squared)
 
     rotated_planet_3d_coeffs = planet_from_star(
         three["p_xx"],
@@ -672,24 +701,34 @@
         three["p_00"],
         x_c,
         y_c,
         z_c,
     )
     rotated_planet_2d_coeffs = planet_2d_coeffs(**rotated_planet_3d_coeffs)
 
-    # return rotated_planet_2d_coeffs
-    r1, r2, _, _, _, _ = _poly_to_parametric_helper(**rotated_planet_2d_coeffs)
+    # # return rotated_planet_2d_coeffs
+    r1, r2, _, _, _, _ = poly_to_parametric_helper(**rotated_planet_2d_coeffs)
     area_seen_by_star = jnp.pi * r1 * r2
 
     return flux_density * area_seen_by_star
 
 
 @jax.jit
 def reflected_phase_curve(
-    sample_radii, sample_thetas, two, three, state, x_c, y_c, z_c
+    sample_radii,
+    sample_thetas,
+    two,
+    three,
+    state,
+    x_c,
+    y_c,
+    z_c,
+    xo=jnp.array([0.0]),
+    yo=jnp.array([0.0]),
+    zo=jnp.array([0.0]),
 ):
     """
     Compute the timeseries of light reflected from  the planet.
 
     This function computes the reflected light from the planet at each time step. It
     assume the planet is a) a Lambertian reflector, b) that the star is a point source
     sending out parallel rays, c) that the :math:`a/R_s >> R_p` (i.e., the distance
@@ -717,14 +756,23 @@
         state (dict):
             A dictionary containing all of the parameters needed to compute the phase
             curve. This includes the planet's orbital parameters, the observer's
             parameters, and the hotspot parameters.
         x_c (Array): The x coordinate of the center of the planet.
         y_c (Array): The y coordinate of the center of the planet.
         z_c (Array): The z coordinate of the center of the planet.
+        xo (Array):
+            An offset to add to the x coordinate of the center of the planet, used when
+            correcting for extended source illuminations. Default is 0.0.
+        yo (Array):
+            An offset to add to the y coordinate of the center of the planet, used when
+            correcting for extended source illuminations. Default is 0.0.
+        zo (Array):
+            An offset to add to the z coordinate of the center of the planet, used when
+            correcting for extended source illuminations. Default is 0.0.
 
 
     Returns:
         Array:
             The timeseries of reflected light from the planet. Each element of the array
             corresponds to the time of the corresponding element in state["times"].
 
@@ -741,14 +789,19 @@
         three["p_xx"] = jnp.ones_like(x_c) * three["p_xx"]
         three["p_xy"] = jnp.ones_like(x_c) * three["p_xy"]
         three["p_xz"] = jnp.ones_like(x_c) * three["p_xz"]
         three["p_yy"] = jnp.ones_like(x_c) * three["p_yy"]
         three["p_yz"] = jnp.ones_like(x_c) * three["p_yz"]
         three["p_zz"] = jnp.ones_like(x_c) * three["p_zz"]
 
+    if x_c.shape != xo.shape:
+        xo = jnp.ones_like(x_c) * xo
+        yo = jnp.ones_like(x_c) * yo
+        zo = jnp.ones_like(x_c) * zo
+
     def scan_func(carry, scan_over):
         (
             rho_xx,
             rho_xy,
             rho_x0,
             rho_yy,
             rho_y0,
@@ -762,18 +815,21 @@
             p_y0,
             p_zz,
             p_z0,
             p_00,
             x_c,
             y_c,
             z_c,
+            xo,
+            yo,
+            zo,
         ) = scan_over
-        x_c = jnp.array([x_c])
-        y_c = jnp.array([y_c])
-        z_c = jnp.array([z_c])
+        x_c = jnp.array([x_c]) - xo
+        y_c = jnp.array([y_c]) - yo
+        z_c = jnp.array([z_c]) - zo
 
         x, y, z = sample_surface(
             sample_radii,
             sample_thetas,
             rho_xx,
             rho_xy,
             rho_x0,
@@ -805,14 +861,17 @@
             p_zz,
             p_z0,
             p_00,
         )
         surface_star_angle = surface_star_cos_angle(n, x_c, y_c, z_c)
         lamb = lambertian_reflection(surface_star_angle, x, y, z)
 
+        mask = ~(((x + xo) ** 2 + (y + yo) ** 2 < 1) & ((z + zo) < 0))
+        lamb = lamb * mask
+
         return None, jnp.sum(lamb) / sample_radii.shape[0]
 
     flux = jax.lax.scan(
         scan_func,
         None,
         (
             two["rho_xx"],
@@ -830,20 +889,47 @@
             three["p_y0"],
             three["p_zz"],
             three["p_z0"],
             three["p_00"],
             x_c,
             y_c,
             z_c,
+            xo,
+            yo,
+            zo,
         ),
     )[1]
 
-    norm = reflected_normalization(two, three, x_c, y_c, z_c)
+    norm = reflected_normalization(two, three, x_c, y_c, z_c, xo, yo, zo)
+
+    return flux * norm * state["albedo"]
 
-    return flux * norm * state["reflected_albedo"]
+
+# still having trouble with this, leaving it for a specific enhancement after 0.1.0
+@jax.jit
+def extended_illumination_reflected_phase_curve(
+    sample_radii, sample_thetas, two, three, state, x_c, y_c, z_c, offsets
+):
+    pass
+    # # def scan_func(carry, scan_over):
+    # #     two, three = scan_over
+    # #     return None, reflected_phase_curve(
+    # #         sample_radii, sample_thetas, two, three, state, x_c, y_c, z_c
+    # #     )
+
+    # # reflected = jax.lax.scan(scan_func,None,(two, three))[1]
+    # # return jnp.mean(reflected, axis=0)
+
+    # xo, yo, zo = offsets[..., 0], offsets[..., 1], offsets[..., 2]
+    # reflected = jax.vmap(
+    #     reflected_phase_curve,
+    #     in_axes=(None, None, 0, 0, None, None, None, None, 0, 0, 0),
+    # )(sample_radii, sample_thetas, two, three, state, x_c, y_c, z_c, xo, yo, zo)
+    # # return jnp.mean(reflected, axis=0)
+    # return reflected
 
 
 ########################################################################################
 # Emission helpers
 ########################################################################################
 
 
@@ -1104,14 +1190,16 @@
     """
 
     # always one time slice at a time
 
     # do this check before you transform into the planet frame
     mask = ~((x**2 + y**2 < 1) & (z < 0))
     x, y, z = jnp.matmul(transform, jnp.array([x, y, z, jnp.ones_like(x)]))
+
+    #
     # correction = emission_squish_correction(x, y, z, r, f1, f2)
 
     # _uncorrected_emission_profile takes the samples on the planet surface and boosts them onto
     # a unit sphere. Had the samples been uniformly distributed on the planet's surface,
     # applying the correction factor to make up for the squishing would be enough. But,
     # we sampled uniformly on the projected disk, not the 3D surface: they don't occupy
     # an area of 4pi, just pi. So, we divide by another factor of 4 here.
@@ -1155,16 +1243,14 @@
     hotspot_latitude,
     hotspot_longitude,
     hotspot_concentration,
 ):
     """
     Compute the emitted intensity at a given point on the planet's surface.
 
-    Corrects for distortion between sphere and ellipsoid, and for viewing geometry.
-
     Args:
         x (Array):
             The x values of the points on the planet's surface in the sky frame
         y (Array):
             The y values of the points on the planet's surface in the sky frame
         z (Array):
             The z values of the points on the planet's surface in the sky frame
@@ -1200,15 +1286,15 @@
     # an area of 4pi, just pi. So, we divide by another factor of 4 here.
 
     # To check this, create a super-concentrated hotspot on a tidally locked planet. The
     # peak emission should be nearly equal to emitted_scale when the hotspot faces the
     # observer, since the rest of the contributions are negligible and the area isn't
     # distorted by viewing geometry
     return jnp.sum(
-        _corrected_emission_profile(
+        corrected_emission_profile(
             x,
             y,
             z,
             transform,
             r,
             f1,
             f2,
@@ -1597,10 +1683,10 @@
             z_c,
         ),
     )[1]
 
     reflected_norm = reflected_normalization(two, three, x_c, y_c, z_c)
 
     return (
-        fluxes[0] * reflected_norm * state["reflected_albedo"],
+        fluxes[0] * reflected_norm * state["albedo"],
         fluxes[1] * state["emitted_scale"],
     )  # the reflected and emitted contributions
```

### Comparing `squishyplanet-0.0.1/squishyplanet/engine/planet_2d.py` & `squishyplanet-0.1.0/squishyplanet/engine/planet_2d.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.0.1/squishyplanet/engine/polynomial_limb_darkened_transit.py` & `squishyplanet-0.1.0/squishyplanet/engine/polynomial_limb_darkened_transit.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 #     ts = jnp.where(jnp.imag(roots) == 0, jnp.real(roots), 999)
 #     xs = jnp.where(ts != 999, (1-ts**2)/(1+ts**2), ts)
 #     ys = jnp.where(ts != 999, 2*ts/(1+ts**2), ts)
 #     return xs, ys
 
 
 @jax.jit
-def parameterize_2d_helper(projected_r1, projected_r2, projected_theta, xc, yc):
+def parameterize_2d_helper(projected_r, projected_f, projected_theta, xc, yc):
     """
     Convert from the alternative sky-projected parameterization to the same format
     used by the 3D parameterization.
 
     A good chunk of the code assumes that the planet's center is determined by the
     orbital elements and that it's outline is derived from an equatorial radius ``r``,
     a z-flattening ``f1``, a y-flattening ``f2``, and two body-centered rotations
@@ -89,56 +89,57 @@
     So, if only doing transits, it is more convenient to parameterize the planet by
     its projected radius in the x and y directions, and the angle of the projected
     ellipse. This function takes in those parameters and returns the same dictionaries
     you'd get if you fed a full 3D parameterization into
     :func:`planet_2d.planet_2d_coeffs`.
 
     Args:
-        projected_r1 (float): The projected "x" radius of the planet.
-        projected_r2 (float): The projected "y" radius of the planet.
+        projected_r (float): The projected "x" radius of the planet.
+        projected_f (float): The flattening of the projected ellipse.
         projected_theta (float): The angle of the projected ellipse.
 
     Returns:
         tuple:
             A tuple of two dictionaries. The first dictionary contains the coefficients
             of the quadratic equation that describes the projected ellipse. The second
             dictionary contains coefficients that describe the parametric form of that
             same ellipse.
 
     """
+    projected_r2 = projected_r * (1 - projected_f)
     cos_t = jnp.cos(projected_theta)
     sin_t = jnp.sin(projected_theta)
 
     two = {
-        "rho_xx": cos_t**2 / projected_r1**2 + sin_t**2 / projected_r2**2,
-        "rho_xy": (2 * cos_t * sin_t) / projected_r1**2
+        "rho_xx": cos_t**2 / projected_r**2 + sin_t**2 / projected_r2**2,
+        "rho_xy": (2 * cos_t * sin_t) / projected_r**2
         - (2 * cos_t * sin_t) / projected_r2**2,
-        "rho_x0": (-2 * cos_t**2 * xc) / projected_r1**2
-        - (2 * cos_t * yc * sin_t) / projected_r1**2
+        "rho_x0": (-2 * cos_t**2 * xc) / projected_r**2
+        - (2 * cos_t * yc * sin_t) / projected_r**2
         + (2 * cos_t * yc * sin_t) / projected_r2**2
         - (2 * xc * sin_t**2) / projected_r2**2,
-        "rho_yy": cos_t**2 / projected_r2**2 + sin_t**2 / projected_r1**2,
+        "rho_yy": cos_t**2 / projected_r2**2 + sin_t**2 / projected_r**2,
         "rho_y0": (-2 * cos_t**2 * yc) / projected_r2**2
-        - (2 * cos_t * xc * sin_t) / projected_r1**2
+        - (2 * cos_t * xc * sin_t) / projected_r**2
         + (2 * cos_t * xc * sin_t) / projected_r2**2
-        - (2 * yc * sin_t**2) / projected_r1**2,
-        "rho_00": (cos_t**2 * xc**2) / projected_r1**2
+        - (2 * yc * sin_t**2) / projected_r**2,
+        "rho_00": (cos_t**2 * xc**2) / projected_r**2
         + (cos_t**2 * yc**2) / projected_r2**2
-        + (2 * cos_t * xc * yc * sin_t) / projected_r1**2
+        + (2 * cos_t * xc * yc * sin_t) / projected_r**2
         - (2 * cos_t * xc * yc * sin_t) / projected_r2**2
-        + (yc**2 * sin_t**2) / projected_r1**2
+        + (yc**2 * sin_t**2) / projected_r**2
         + (xc**2 * sin_t**2) / projected_r2**2,
     }
 
     para = {
-        "c_x1": projected_r1 * cos_t,
-        "c_x2": -projected_r2 * sin_t,
+        "c_x1": jnp.ones_like(xc) * (projected_r * cos_t),
+        "c_x2": jnp.ones_like(xc) * (-projected_r2 * sin_t),
         "c_x3": xc,
-        "c_y1": projected_r1 * sin_t,
-        "c_y2": projected_r2 * cos_t,
+        "c_y1": jnp.ones_like(xc) * (projected_r * sin_t),
+        "c_y2": jnp.ones_like(xc) * (projected_r2 * cos_t),
         "c_y3": yc,
     }
 
     return two, para
 
 
 @jax.jit
@@ -392,15 +393,15 @@
 
     solution_vec = jnp.zeros(g_coeffs.shape[0])
     solution_vec = solution_vec.at[0].set(s0)
     solution_vec = solution_vec.at[1].set(s1)
     return solution_vec
 
 
-@partial(jax.jit, static_argnums=(1,))
+@partial(jax.jit, static_argnames=("parameterize_with_projected_ellipse",))
 def lightcurve(state, parameterize_with_projected_ellipse):
     """
     The main function for computing a transit light curve.
 
     This function will return a 1-D array representing the flux recieved from the star,
     where each entry corresponds to a time in the input `state` dictionary. It first
     transforms the `state` into the implicit 3D surface of the planet, the implicit 2D
@@ -456,33 +457,33 @@
     normalization_constant = 1 / (jnp.pi * (g_coeffs[0] + (2 / 3) * g_coeffs[1]))
 
     # cartesian position of the planet at each timestep
     positions = skypos(**state)
 
     if parameterize_with_projected_ellipse:
         two, para = parameterize_2d_helper(
-            state["projected_r1"],
-            state["projected_r2"],
+            state["projected_r"],
+            state["projected_f"],
             state["projected_theta"],
             positions[0, :],
             positions[1, :],
         )
-
-        largest_r = jnp.max(jnp.array([state["projected_r1"], state["projected_r2"]]))
+        r2 = state["projected_r"] * (1 - state["projected_f"])
+        largest_r = jnp.max(jnp.array([state["projected_r"], r2]))
 
     else:
+        state["prec"] = jnp.where(state["tidally_locked"], state["f"], state["prec"])
+
         # the coefficients of the implicit 3d surface
         three = planet_3d_coeffs(**state)
         # the coefficients of the implicit 2d surface
         two = planet_2d_coeffs(**three)
         # the coefficients of the parametric projected ellipse
         para = poly_to_parametric(**two)
 
-        state["prec"] = jnp.where(state["tidally_locked"], state["f"], state["prec"])
-
         largest_r = state["r"]
 
     possibly_in_transit = (
         positions[0, :] ** 2 + positions[1, :] ** 2 <= (1.0 + largest_r * 1.1) ** 2
     ) * (positions[2, :] > 0)
 
     def not_on_limb(X):
```

### Comparing `squishyplanet-0.0.1/squishyplanet/oblate_system.py` & `squishyplanet-0.1.0/squishyplanet/oblate_system.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,29 +4,40 @@
 import jax.numpy as jnp
 
 import copy
 from functools import partial
 import pprint
 import matplotlib.pyplot as plt
 
-from squishyplanet.engine.planet_3d import planet_3d_coeffs
+from squishyplanet.engine.planet_3d import (
+    planet_3d_coeffs,
+    extended_illumination_offsets,
+    planet_3d_coeffs_extended_illumination,
+)
 from squishyplanet.engine.planet_2d import planet_2d_coeffs
-from squishyplanet.engine.parametric_ellipse import poly_to_parametric
+from squishyplanet.engine.parametric_ellipse import (
+    poly_to_parametric_helper,
+    poly_to_parametric,
+)
 from squishyplanet.engine.greens_basis_transform import generate_change_of_basis_matrix
 from squishyplanet.engine.kepler import kepler, skypos
-from squishyplanet.engine.polynomial_limb_darkened_transit import lightcurve
+from squishyplanet.engine.polynomial_limb_darkened_transit import (
+    lightcurve,
+    parameterize_2d_helper,
+)
 from squishyplanet.engine.phase_curve_utils import (
     pre_squish_transform,
     generate_sample_radii_thetas,
     sample_surface,
     planet_surface_normal,
     surface_star_cos_angle,
     lambertian_reflection,
     corrected_emission_profile,
     reflected_phase_curve,
+    extended_illumination_reflected_phase_curve,
     emission_phase_curve,
     phase_curve,
     stellar_ellipsoidal_variations,
     stellar_doppler_variations,
 )
 
 
@@ -91,15 +102,15 @@
             planet about an axis that's aligned with its orbit normal and runs through
             the center of the planet (e.g., if obliq=0, it would set the planet's
             instantaneous rotational phase, and if obliq :math:`\\neq` 0, it would set
             the "season" of the northern hemisphere at periastron passage.)
         r (float, [Rstar], default=None):
             The equatorial radius of the planet. This will always be the largest of the
             3 axes of the triaxial ellipsoid. Either this or the entire set of
-            ``projected_r1``, ``projected_r2``, and ``projected_theta`` must be
+            ``projected_r``, ``projected_f``, and ``projected_theta`` must be
             provided.
         f1 (float, [Dimensionless], default=0.0):
             The fractional difference between the (longest) equatorial and polar radii
             of the planet. This is defined as :math:`(R_{eq} - R_{pol}) / R_{eq}`.
         f2 (float, [Dimensionless], default=0.0):
             The fractional difference between long and short radii of the ellipse that
             defines the equator of the planet. Defined similarly to f1.
@@ -121,41 +132,48 @@
             sense: 0 is the north pole, :math:`\pi/2` is the equator, and :math:`\pi` is
             the south pole.
         hotspot_longitude (float, [Radian], default=0.0):
             The longitude of a potential hotspot on the planet.
         hotspot_concentration (float, default=0.2):
             The "concentration" of the hotspot. This is the :math:`\kappa` parameter in
             the von Mises-Fisher distribution that describes the hotspot.
-        reflected_albedo (float, default=1.0):
+        albedo (float, default=1.0):
             The (spatialy uniform) albedo of the planet. This is the fraction of light
             that is reflected, though the directional-dependent scattering is dictated
             by Lambert's cosine law.
-        emitted_scale (float, default=1.0):
-            The total emitted flux of the planet, in units of un-occulted stellar flux.
-            The von Mises-Fisher distribution integrates to 1, and this factor scales
-            the resulting emission profile.
+        emitted_scale (float, default=1e-5):
+            A scale factor that sets the amplitude of the the emitted flux of the
+            planet.
         systematic_trend_coeffs (array-like, default=jnp.array([0.0,0.0])):
             The coefficients that determine the polynomial trend in time added to the
             lightcurves. Used to optionally model long-term drifts in observed data.
         log_jitter (float, default=-10):
             The log of the "jitter" term included in likelihood calculations. The jitter
             is added in quadrature to the provided uncertainties to account for any
             unmodeled noise in the data.
-        projected_r1 (float, [Rstar], default=0.0):
+        projected_r (float, [Rstar], default=0.0):
             The length of the semi-major axis of the projected ellipse. This is only
             relevant if ``parameterize_with_projected_ellipse`` is set to ``True``,
             which will override ``r``, ``f1``, ``f2``, ``obliq``, and ``prec``.
-        projected_r2 (float, [Rstar], default=0.0):
-            The length of the semi-minor axis of the projected ellipse. This is only
-            relevant if ``parameterize_with_projected_ellipse`` is set to ``True``,
-            which will override ``r``, ``f1``, ``f2``, ``obliq``, and ``prec``.
+        projected_f (float, [Dimensionless], default=0.0):
+            The flattening value of the projected ellipse. This is only relevant if
+            ``parameterize_with_projected_ellipse`` is set to ``True``, which will
+            override ``r``, ``f1``, ``f2``, ``obliq``, and ``prec``.
         projected_theta (float, [Radian], default=0.0):
             The angle of the semi-major axis of the projected ellipse. This is only
             relevant if ``parameterize_with_projected_ellipse`` is set to ``True``,
             which will override ``r``, ``f1``, ``f2``, ``obliq``, and ``prec``.
+        extended_illumination_npts (int, default=1):
+            The number of points used to sample the star's projected disk as seen by
+            the planet when calculating the reflected flux and accounting for the star's
+            extended size. Closely follows the implementation in ``starry``,
+            specifically Sec. 4.1 of `Luger et al. 2022
+            <https://ui.adsabs.harvard.edu/abs/2022AJ....164....4L/abstract>`_.
+            IMPLEMENTATION IS INCOMPLETE, WILL RAISE A NOTIMPLEMENTEDERROR IF SET TO
+            ANYTHING OTHER THAN 1.
         tidally_locked (bool, default=True):
             Whether the planet is tidally locked to the star. If ``True``, then ``prec``
             will always be set equal to the true anomaly, meaning the same face of the
             planet will always face the star.
         compute_reflected_phase_curve (bool, default=False):
             Whether to include flux reflected by the planet when calling
             :func:`lightcurve`.
@@ -169,15 +187,16 @@
             peaks per orbit.
         compute_stellar_doppler_variations (bool, default=False):
             Whether to include stellar doppler variations in the light curve. This
             captures the effects of the star's radial velocity changing and boosting the
             total flux/pushing some flux into/out of the bandpass of the observation.
             Here, it is modeled as a simple sinusoidal variation with 2 peaks per orbit.
         parameterize_with_projected_ellipse (bool, default=False):
-
+            Whether to parameterize the planet as a projected ellipse rather than a
+            triaxial ellipsoid. If ``True``, then ``projected_r``, ``projected_f``,
         phase_curve_nsamples (int, default=50_000):
             The number of random samples of the planet's surface to draw when performing
             Monte Carlo estimates of the emitted/reflected flux. A larger number will
             increase the resolution/shrink the error of the estimate but result in
             longer computation times.
         random_seed (int, default=0):
             A random seed used for the Monte Carlo integrals in the phase curve. This
@@ -187,14 +206,34 @@
         data (array-like, default=jnp.array([1.0])):
             The observed data to compare to the light curve. Must be the same length as
             ``times``. Only needed if calling :func:`loglike`.
         uncertainties (array-like, default=jnp.array([0.01])):
             The uncertainties on the observed data. Must be the same length as ``data``,
             even if the errors are homoskedastic. Only needed if calling
             :func:`loglike`.
+        exposure_time (float, [Days], default=0.0):
+            The length of each exposure in the light curve, used to correct for finite
+            integration times if ``oversample`` is set to a value greater than 1.
+            Important: the finite exposure time correction procedure assumes that the
+            given times correspond to the **midpoints** of each exposure, not the
+            *start* or *end*. No checks are made to ensure that it is shorter than the
+            minimum time difference between the provided times.
+        oversample (int, default=1):
+            The factor by which to oversample the light curve to partially compensate
+            for finite-time integrations. The overdense lightcurve is then binned down
+            to the original provided times. See e.g. `Kipping 2010
+            <https://ui.adsabs.harvard.edu/abs/2010MNRAS.408.1758K/abstract>`_, "Binning
+            is Sinning" for more. Must be a positive integer. Will be rounded up to
+            nearest odd number.
+        oversample_correction_order (int, default=2):
+            After oversampling the light curve, how do you want to integrate over the
+            exposure time to get the final binned light curve? This follows ``starry``'s
+            treatment very closely: 0 is a centered Riemann sum like in Kipping 2010,
+            1 is a trapezoidal rule, and 2 is Simpson's rule. Must be one of those
+            values.
 
     """
 
     def __init__(
         self,
         times=None,
         t_peri=None,
@@ -209,108 +248,161 @@
         r=None,
         f1=0.0,
         f2=0.0,
         ld_u_coeffs=jnp.array([0.0, 0.0]),
         hotspot_latitude=0.0,
         hotspot_longitude=0.0,
         hotspot_concentration=0.2,
-        reflected_albedo=1.0,
-        emitted_scale=1e-6,
+        albedo=1.0,
+        emitted_scale=1e-5,
         stellar_ellipsoidal_alpha=1e-6,
         stellar_doppler_alpha=1e-6,
         systematic_trend_coeffs=jnp.array([0.0, 0.0]),
         log_jitter=-10,
-        projected_r1=0.0,
-        projected_r2=0.0,
+        projected_r=0.0,
+        projected_f=0.0,
         projected_theta=0.0,
+        extended_illumination_npts=1,
         tidally_locked=True,
         compute_reflected_phase_curve=False,
         compute_emitted_phase_curve=False,
         compute_stellar_ellipsoidal_variations=False,
         compute_stellar_doppler_variations=False,
         parameterize_with_projected_ellipse=False,
         phase_curve_nsamples=50_000,
         random_seed=0,
         data=jnp.array([1.0]),
         uncertainties=jnp.array([0.01]),
+        exposure_time=0.0,
+        oversample=1,
+        oversample_correction_order=2,
     ):
 
-        state_keys = [
-            "times",
-            "t_peri",
-            "period",
-            "a",
-            "e",
-            "i",
-            "Omega",
-            "omega",
-            "obliq",
-            "prec",
-            "r",
-            "f1",
-            "f2",
-            "ld_u_coeffs",
-            "hotspot_latitude",
-            "hotspot_longitude",
-            "hotspot_concentration",
-            "reflected_albedo",
-            "emitted_scale",
-            "stellar_ellipsoidal_alpha",
-            "stellar_doppler_alpha",
-            "systematic_trend_coeffs",
-            "log_jitter",
-            "projected_r1",
-            "projected_r2",
-            "projected_theta",
-            "tidally_locked",
-            "compute_reflected_phase_curve",
-            "compute_emitted_phase_curve",
-            "compute_stellar_ellipsoidal_variations",
-            "compute_stellar_doppler_variations",
-            "parameterize_with_projected_ellipse",
-            "phase_curve_nsamples",
-            "random_seed",
-            "data",
-            "uncertainties",
-        ]
+        #######################################################################
+        # setup
+        #######################################################################
+
+        state_keys = list(locals().keys())
+        state_keys.remove("self")
 
         state = {}
         for key in state_keys:
             state[key] = locals()[key]
         self._state = state
 
         self._validate_inputs()
 
+        #######################################################################
+        # 1-time calculations
+        #######################################################################
+
         # necessary for all light curves
         self._state["greens_basis_transform"] = generate_change_of_basis_matrix(
             len(self._state["ld_u_coeffs"])
         )
 
+        # for oversampling
+        if self._state["oversample"] > 1:
+
+            self._state["oversample"] += 1 - self._state["oversample"] % 2
+            self._state["stencil"] = jnp.ones(self._state["oversample"])
+
+            # Construct the exposure time integration stencil
+            if self._state["oversample_correction_order"] == 0:
+                dt = jnp.linspace(-0.5, 0.5, 2 * self._state["oversample"] + 1)[1:-1:2]
+            elif self._state["oversample_correction_order"] == 1:
+                dt = jnp.linspace(-0.5, 0.5, self._state["oversample"])
+                self._state["stencil"] = self._state["stencil"].at[1:-1].set(2)
+            elif self._state["oversample_correction_order"] == 2:
+                dt = jnp.linspace(-0.5, 0.5, self._state["oversample"])
+                self._state["stencil"] = self._state["stencil"].at[1:-1:2].set(4)
+                self._state["stencil"] = self._state["stencil"].at[2:-1:2].set(2)
+
+            self._state["stencil"] = self._state["stencil"] / jnp.sum(
+                self._state["stencil"]
+            )
+
+            dt = self._state["exposure_time"] * dt
+            t = self._state["times"][:, None] + dt[None, :]
+            t = t.reshape(-1)
+            self._state["times"] = t
+
+        else:
+            self._state["times"] = self._state["times"]
+            self._state["stencil"] = (
+                None  # never used in this case, but to keep the state consistent
+            )
+
+        # # for extended illumination reflection curves
+        # actually, still having trouble with this, so setting aside for now--
+        # leaving it for a specific enhancement after 0.1.0
+        if self._state["compute_reflected_phase_curve"] > 1:
+            raise NotImplementedError(
+                "Extended illumination reflection curves are not yet implemented"
+            )
+        # # based on starry._core.core.py's OpsReflected(OpsYlm) class
+        # # create a grid of points uniformly distributed on the projected disk of the
+        # # sta from an observer along the z-axis
+        # N = int(2 + jnp.sqrt(self._state["extended_illumination_npts"] * 4 / jnp.pi))
+
+        # # note these points will be squished closer together during calculations to
+        # # account for the a-dependent extent of the star from the planet's perspective
+        # dx = jnp.linspace(-1 + 1e-12, 1 - 1e-12, N)
+        # dx, dy = jnp.meshgrid(dx, dx)
+        # # dz = jnp.sqrt(1 - dx**2 - dy**2)
+        # dz = 1 - dx**2 - dy**2
+        # source_dx = dx[dz > 0].flatten()
+        # source_dy = dy[dz > 0].flatten()
+        # source_dz = dz[dz > 0].flatten()
+        # pts = jnp.array([source_dx, source_dy, jnp.sqrt(source_dz)]).T
+        # self._state["extended_illumination_points"] = pts
+        # self._state["extended_illumination_npts"] = len(pts)
+
         # everything below here is just an instantaneous snapshot mostly for plotting,
         # these will all vary with different parameter inputs
         time_deltas = self._state["times"] - self._state["t_peri"]
         mean_anomalies = 2 * jnp.pi * time_deltas / state["period"]
         true_anomalies = kepler(mean_anomalies, state["e"])
         self._state["f"] = true_anomalies
 
         if self._state["tidally_locked"]:
             self._state["prec"] = self._state["f"]
 
         positions = skypos(**state)
-        state["x_c"] = positions[0, :]
-        state["y_c"] = positions[1, :]
-        state["z_c"] = positions[2, :]
-
-        self._coeffs_3d = planet_3d_coeffs(**self._state)
-        for key in self._coeffs_3d.keys():
-            if self._coeffs_3d[key].shape[0] == ():
-                self._coeffs_3d[key] = jnp.array([self._coeffs_3d[key]])
+        self._state["x_c"] = positions[0, :]
+        self._state["y_c"] = positions[1, :]
+        self._state["z_c"] = positions[2, :]
 
-        self._coeffs_2d = planet_2d_coeffs(**self._coeffs_3d)
-        self._para_coeffs_2d = poly_to_parametric(**self._coeffs_2d)
+        if not self._state["parameterize_with_projected_ellipse"]:
+            self._coeffs_3d = planet_3d_coeffs(**self._state)
+            for key in self._coeffs_3d.keys():
+                if self._coeffs_3d[key].shape[0] == ():
+                    self._coeffs_3d[key] = jnp.array([self._coeffs_3d[key]])
+
+            self._coeffs_2d = planet_2d_coeffs(**self._coeffs_3d)
+            self._para_coeffs_2d = poly_to_parametric(**self._coeffs_2d)
+
+            r1, r2, _, _, _, _ = poly_to_parametric_helper(**self._coeffs_2d)
+            area = jnp.pi * r1 * r2
+            effective_r = jnp.sqrt(area / jnp.pi)
+            self._state["effective_projected_r"] = effective_r
+        else:
+            self._coeffs_3d = {}
+            self._coeffs_2d, self._para_coeffs_2d = parameterize_2d_helper(
+                projected_r=self._state["projected_r"],
+                projected_f=self._state["projected_f"],
+                projected_theta=self._state["projected_theta"],
+                xc=self._state["x_c"],
+                yc=self._state["y_c"],
+            )
+            r1 = self._state["projected_r"]
+            r2 = r1 * (1 - self._state["projected_f"])
+            area = jnp.pi * r1 * r2
+            effective_r = jnp.sqrt(area / jnp.pi)
+            self._state["effective_projected_r"] = effective_r
 
     def __repr__(self):
         s = pprint.pformat(self.state)
         return f"OblateSystem(\n{s}\n)"
 
     @property
     def state(self):
@@ -323,20 +415,33 @@
         which to generate the lightcurve, just define a new system with those values.
 
         Returns:
             dict:
             A dictionary of all the parameters of the system, including those specified
             by the user, default values, and those calculated by combinations of the
             two.
+
         """
-        return self._state
+
+        # we internally changed "times" if oversample > 1, but we alwasy bin it back
+        # down to the original times, so we can undo that expansion here
+        s = copy.deepcopy(self._state)
+        if s["oversample"] > 1:
+            s["times"] = (
+                s["times"].reshape(-1, s["oversample"]) * s["stencil"][None, :]
+            ).sum(axis=1)
+        return s
 
     def _validate_inputs(self):
         for key, val in self._state.items():
             if type(val) == type(None):
+                if key == "r":
+                    if self._state["parameterize_with_projected_ellipse"]:
+                        self._state["r"] = 0.0
+                        continue
                 raise ValueError(f"'{key}' is a required parameter")
 
         self._state["ld_u_coeffs"] = jnp.array(self._state["ld_u_coeffs"])
         assert (
             self._state["ld_u_coeffs"].shape[0] >= 2
         ), "ld_u_coeffs must have at least 2 (even if higher-order terms are 0)"
         assert (
@@ -353,14 +458,18 @@
                 (key == "times")
                 | (key == "ld_u_coeffs")
                 | (key == "phase_curve_nsamples")
                 | (key == "random_seed")
                 | (key == "data")
                 | (key == "uncertainties")
                 | (key == "systematic_trend_coeffs")
+                | (key == "exposure_time")
+                | (key == "oversample")
+                | (key == "oversample_correction_order")
+                | (key == "extended_illumination_npts")
             ):
                 continue
             elif type(self._state[key]) == bool:
                 continue
 
             if (type(self._state[key]) == float) | (type(self._state[key]) == int):
                 self._state[key] = jnp.array([self._state[key]])
@@ -377,52 +486,66 @@
                     shapes.append(self._state[key].shape[0])
         if len(jnp.unique(jnp.array(shapes))) > 2:
             raise ValueError(
                 "All parameters must be scalars or arrays of the same shape."
             )
 
         if self._state["parameterize_with_projected_ellipse"]:
-            assert self._state["projected_r1"] > 0, (
-                "projected_r1 must be greater than 0 if "
+            assert self._state["projected_r"] > 0, (
+                "projected_r must be greater than 0 if "
                 "parameterize_with_projected_ellipse is True"
             )
-            assert self._state["projected_r2"] > 0, (
-                "projected_r2 must be greater than 0 if "
-                "parameterize_with_projected_ellipse is True"
-            )
-            assert (
-                not self._state["compute_reflected_phase_curve"]
-                & self._state["compute_emitted_phase_curve"]
-                & self._state["compute_stellar_ellipsoidal_variations"]
-                & self._state["compute_stellar_doppler_variations"],
-                (
-                    "parameterize_with_projected_ellipse is incompatible with "
-                    "phase curve calculations"
-                ),
+            assert not (
+                self._state["compute_reflected_phase_curve"]
+                | self._state["compute_emitted_phase_curve"]
+                | self._state["compute_stellar_ellipsoidal_variations"]
+                | self._state["compute_stellar_doppler_variations"]
+            ), (
+                "parameterize_with_projected_ellipse is incompatible with phase"
+                "curve calculations"
             )
+
             assert self._state["tidally_locked"] == False, (
                 "parameterize_with_projected_ellipse is incompatible with "
                 "tidally_locked=True"
             )
 
+        assert (self._state["oversample_correction_order"] in [0, 1, 2]) & (
+            type(self._state["oversample_correction_order"]) == int
+        ), "oversample_correction_order must be 0, 1, or 2"
+
+        assert self._state["oversample"] > 0, "oversample must be greater than 0"
+
+        if self._state["oversample"] > 1:
+            assert (
+                self._state["exposure_time"] is not None
+            ), "exposure_time must be provided if oversample > 1"
+
+        if self._state["compute_stellar_ellipsoidal_variations"]:
+            assert (
+                self._state["e"] == 0.0
+            ), "Stellar ellipsoidal variations are only valid for circular orbits"
+
+        if self._state["compute_stellar_doppler_variations"]:
+            assert (
+                self._state["e"] == 0.0
+            ), "Stellar doppler variations are only valid for circular orbits"
+
     def _illustrate_helper(self, times=None, true_anomalies=None, nsamples=50_000):
 
         if (times is not None) & (true_anomalies is not None):
             raise ValueError("Provide either times or true anomalies but not both")
 
         if times is not None:
             time_deltas = times - self._state["t_peri"]
             mean_anomalies = 2 * jnp.pi * time_deltas / self._state["period"]
             true_anomalies = kepler(mean_anomalies, self._state["e"])
         elif true_anomalies is not None:
             pass
         else:
-            # true_anomalies = jnp.array(
-            #     [0.0, jnp.pi / 2, jnp.pi, 3 * jnp.pi / 2]
-            # )
             true_anomalies = jnp.array([jnp.pi / 2])
 
         if (type(true_anomalies) == float) | (type(true_anomalies) == int):
             true_anomalies = jnp.array([true_anomalies])
 
         # the trace of the orbit
         fs = jnp.linspace(0, 2 * jnp.pi, 300)
@@ -436,83 +559,112 @@
         )
         behind_star = (
             (orbit_positions[0, :] ** 2 + orbit_positions[1, :] ** 2) < 1
         ) & (orbit_positions[2, :] < 0)
         orbit_positions = orbit_positions.at[:, behind_star].set(jnp.nan)
 
         original_state = copy.deepcopy(self._state)
+        original_3d_coeffs = copy.deepcopy(self._coeffs_3d)
+        original_2d_coeffs = copy.deepcopy(self._coeffs_2d)
+        original_para_coeffs_2d = copy.deepcopy(self._para_coeffs_2d)
+
         X_outline = []
         Y_outline = []
         Xs = []
         Ys = []
         Reflection = []
         Emission = []
         for i in range(len(true_anomalies)):
 
             # all of these could just be done in one go,
             # but bookkeeping was easier this way
             self._state["f"] = jnp.array([true_anomalies[i]])
             if self._state["tidally_locked"]:
                 self._state["prec"] = self._state["f"]
-            self._coeffs_3d = planet_3d_coeffs(**self._state)
-            self._coeffs_2d = planet_2d_coeffs(**self._coeffs_3d)
-            self._para_coeffs_2d = poly_to_parametric(**self._coeffs_2d)
+            # self._coeffs_3d = planet_3d_coeffs(**self._state)
+            # self._coeffs_2d = planet_2d_coeffs(**self._coeffs_3d)
+            # self._para_coeffs_2d = poly_to_parametric(**self._coeffs_2d)
             positions = skypos(**self._state)
             self._state["x_c"] = positions[0, :]
             self._state["y_c"] = positions[1, :]
             self._state["z_c"] = positions[2, :]
+            if not self._state["parameterize_with_projected_ellipse"]:
+                self._coeffs_3d = planet_3d_coeffs(**self._state)
+                for key in self._coeffs_3d.keys():
+                    if self._coeffs_3d[key].shape[0] == ():
+                        self._coeffs_3d[key] = jnp.array([self._coeffs_3d[key]])
+
+                self._coeffs_2d = planet_2d_coeffs(**self._coeffs_3d)
+                self._para_coeffs_2d = poly_to_parametric(**self._coeffs_2d)
+
+            else:
+                self._coeffs_3d = {}
+                self._coeffs_2d, self._para_coeffs_2d = parameterize_2d_helper(
+                    projected_r=self._state["projected_r"],
+                    projected_f=self._state["projected_f"],
+                    projected_theta=self._state["projected_theta"],
+                    xc=self._state["x_c"],
+                    yc=self._state["y_c"],
+                )
 
             # the boundary of the planet
             thetas = jnp.linspace(0, 2 * jnp.pi, 200)
             x_outline = (
                 self._para_coeffs_2d["c_x1"] * jnp.cos(thetas)
                 + self._para_coeffs_2d["c_x2"] * jnp.sin(thetas)
                 + self._para_coeffs_2d["c_x3"]
             )
             y_outline = (
                 self._para_coeffs_2d["c_y1"] * jnp.cos(thetas)
                 + self._para_coeffs_2d["c_y2"] * jnp.sin(thetas)
                 + self._para_coeffs_2d["c_y3"]
             )
 
-            # the phase curve bits
-            sample_radii, sample_thetas = generate_sample_radii_thetas(
-                jax.random.key(0), jnp.arange(nsamples)
-            )
-            x, y, z = sample_surface(
-                sample_radii,
-                sample_thetas,
-                **self._coeffs_2d,
-                **self._coeffs_3d,
-            )
-
-            # the reflected brightness profile
-            normals = planet_surface_normal(x, y, z, **self._coeffs_3d)
-            star_cos_ang = surface_star_cos_angle(
-                normals,
-                self._state["x_c"],
-                self._state["y_c"],
-                self._state["z_c"],
-            )
-            reflection = lambertian_reflection(star_cos_ang, x, y, z)
-
-            # the emitted brightness profile
-            # need to take the first index since you aren't scanning here
-            transform = pre_squish_transform(**self._state)[0]
-            emission = corrected_emission_profile(
-                x,
-                y,
-                z,
-                transform,
-                **self._state,
-            )
-
-            behind_star = ((x**2 + y**2) < 1) & (z < 0)
-            reflection = jnp.where(behind_star, jnp.nan, reflection)
-            emission = jnp.where(behind_star, jnp.nan, emission)
+            if not self._state["parameterize_with_projected_ellipse"]:
+                # the phase curve bits
+                sample_radii, sample_thetas = generate_sample_radii_thetas(
+                    jax.random.key(0), jnp.arange(nsamples)
+                )
+                x, y, z = sample_surface(
+                    sample_radii,
+                    sample_thetas,
+                    **self._coeffs_2d,
+                    **self._coeffs_3d,
+                )
+
+                # the reflected brightness profile
+                normals = planet_surface_normal(x, y, z, **self._coeffs_3d)
+                star_cos_ang = surface_star_cos_angle(
+                    normals,
+                    self._state["x_c"],
+                    self._state["y_c"],
+                    self._state["z_c"],
+                )
+                reflection = lambertian_reflection(star_cos_ang, x, y, z)
+
+                # the emitted brightness profile
+                # need to take the first index since you aren't scanning here
+                transform = pre_squish_transform(**self._state)[0]
+                emission = corrected_emission_profile(
+                    x,
+                    y,
+                    z,
+                    transform,
+                    **self._state,
+                )
+
+                behind_star = ((x**2 + y**2) < 1) & (z < 0)
+                reflection = jnp.where(behind_star, jnp.nan, reflection)
+                emission = jnp.where(behind_star, jnp.nan, emission)
+
+            else:
+                x = jnp.nan
+                y = jnp.nan
+                reflection = jnp.nan
+                emission = jnp.nan
 
             X_outline.append(x_outline)
             Y_outline.append(y_outline)
             Xs.append(x)
             Ys.append(y)
             Reflection.append(reflection)
             Emission.append(emission)
@@ -525,14 +677,18 @@
         Emission = jnp.array(Emission)
 
         # behind_star = ((Xs ** 2 + Ys ** 2) < 1)
         # Reflection = jnp.where(Reflection == 0, jnp.nan, Reflection)
         # Emission = jnp.where(Emission == 0, jnp.nan, Emission)
 
         self._state = original_state
+        self._coeffs_3d = original_3d_coeffs
+        self._coeffs_2d = original_2d_coeffs
+        self._para_coeffs_2d = original_para_coeffs_2d
+
         return {
             "orbit_positions": orbit_positions,
             "planet_x_outlines": X_outline,
             "planet_y_outlines": Y_outline,
             "sample_xs": Xs,
             "sample_ys": Ys,
             "reflected_intensity": Reflection,
@@ -601,14 +757,15 @@
 
         Returns:
             None:
             This method is used for its side effects of displaying a plot, not for its
             return value.
 
         """
+
         if emitted:
             assert (
                 reflected == False
             ), "Can't illustrate both reflected and emitted flux"
         if reflected:
             assert emitted == False, "Can't illustrate both reflected and emitted flux"
 
@@ -623,15 +780,15 @@
             im_center_y = 0
         else:
             im_center_x = jnp.mean(info["planet_x_outlines"])
             im_center_y = jnp.mean(info["planet_y_outlines"])
 
         star = plt.Circle((0, 0), 1, color="black", fill=False)
         ax.add_artist(star)
-        if star_fill:
+        if star_fill & (not jnp.all(self._state["ld_u_coeffs"] == 0)):
             # lifted from engine.polynomial_limb_darkened_transit
             u_coeffs = jnp.ones(self._state["ld_u_coeffs"].shape[0] + 1) * (-1)
             u_coeffs = u_coeffs.at[1:].set(self._state["ld_u_coeffs"])
             g_coeffs = jnp.matmul(self._state["greens_basis_transform"], u_coeffs)
             normalization_constant = 1 / (
                 jnp.pi * (g_coeffs[0] + (2 / 3) * g_coeffs[1])
             )
@@ -650,14 +807,17 @@
             Z = jax.vmap(_star_radial_profile)(R.flatten()).reshape(X.shape)
 
             min_val = jnp.max(jnp.array([0, jnp.nanmin(Z)]))
             max_val = jnp.nanmax(Z)
             ax.contourf(
                 X, Y, Z, cmap="copper", levels=jnp.linspace(min_val, max_val, 20)
             )
+        elif star_fill:
+            fill = plt.Circle((0, 0), 1, color="orange", fill=True, alpha=0.5)
+            ax.add_artist(fill)
 
         if orbit:
             ax.plot(
                 info["orbit_positions"][0, :],
                 info["orbit_positions"][1, :],
                 color="black",
                 ls="--",
@@ -713,17 +873,18 @@
         Args:
             r (float or array-like):
                 The radius at which to compute the limb darkening profile. Must be
                 between 0 and 1.
 
         Returns:
             Array:
-            The limb darkening profile of the star at the given radius.
+                The limb darkening profile of the star at the given radius.
 
         """
+
         u_coeffs = jnp.ones(self._state["ld_u_coeffs"].shape[0] + 1) * (-1)
         u_coeffs = u_coeffs.at[1:].set(self._state["ld_u_coeffs"])
         g_coeffs = jnp.matmul(self._state["greens_basis_transform"], u_coeffs)
 
         # total flux from the star. 1/eq. 28 in Agol, Luger, and Foreman-Mackey 2020
         normalization_constant = 1 / (jnp.pi * (g_coeffs[0] + (2 / 3) * g_coeffs[1]))
 
@@ -773,26 +934,33 @@
                     "r" : 0.1,
                     "compute_reflected_phase_curve" : True,
                     "compute_emitted_phase_curve" : True,
                     "emitted_scale" : 1e-5,
                 }
             >>> system = OblateSystem(**state)
             >>> system.lightcurve()
+
         """
+
         return _lightcurve(
             compute_reflected_phase_curve=self._state["compute_reflected_phase_curve"],
             compute_emitted_phase_curve=self._state["compute_emitted_phase_curve"],
             compute_stellar_ellipsoidal_variations=self._state[
                 "compute_stellar_ellipsoidal_variations"
             ],
             compute_stellar_doppler_variations=self._state[
                 "compute_stellar_doppler_variations"
             ],
+            parameterize_with_projected_ellipse=self._state[
+                "parameterize_with_projected_ellipse"
+            ],
+            oversample=self._state["oversample"],
             random_seed=self._state["random_seed"],
             phase_curve_nsamples=self._state["phase_curve_nsamples"],
+            extended_illumination_npts=self._state["extended_illumination_npts"],
             state=self._state,
             params=params,
         )
 
     def loglike(self, params={}):
         """
         Compute the log likelihood of the system given the observed data and some set of
@@ -819,53 +987,71 @@
             compute_emitted_phase_curve=self._state["compute_emitted_phase_curve"],
             compute_stellar_ellipsoidal_variations=self._state[
                 "compute_stellar_ellipsoidal_variations"
             ],
             compute_stellar_doppler_variations=self._state[
                 "compute_stellar_doppler_variations"
             ],
+            parameterize_with_projected_ellipse=self._state[
+                "parameterize_with_projected_ellipse"
+            ],
+            oversample=self._state["oversample"],
             random_seed=self._state["random_seed"],
             phase_curve_nsamples=self._state["phase_curve_nsamples"],
+            extended_illumination_npts=self._state["extended_illumination_npts"],
             state=self._state,
             params=params,
         )
 
 
 @partial(
     jax.jit,
     static_argnums=(
         0,
         1,
         2,
         3,
         4,
         5,
+        6,
+        7,
+        8,
     ),
 )
 def _lightcurve(
     compute_reflected_phase_curve,
     compute_emitted_phase_curve,
     compute_stellar_ellipsoidal_variations,
     compute_stellar_doppler_variations,
+    parameterize_with_projected_ellipse,
+    oversample,
     random_seed,
     phase_curve_nsamples,
+    extended_illumination_npts,
     state,
     params,
 ):
     # always compute the primary transit and trend
     for key in params.keys():
         state[key] = params[key]
-    transit = lightcurve(state, state["parameterize_with_projected_ellipse"])
+    transit = lightcurve(state, parameterize_with_projected_ellipse)
     trend = jnp.polyval(state["systematic_trend_coeffs"], state["times"])
 
     # if you don't want any phase curve stuff, you're done
     if (not compute_reflected_phase_curve) & (not compute_emitted_phase_curve) and (
         not compute_stellar_doppler_variations
     ) & (not compute_stellar_ellipsoidal_variations):
-        return transit + trend
+        oversampled_curve = transit + trend
+        if oversample > 1:
+            c = (
+                oversampled_curve.reshape(-1, oversample) * state["stencil"][None, :]
+            ).sum(axis=1)
+        else:
+            c = oversampled_curve
+        return c
 
     ######################################################
     # compute the planet's contribution to the phase curve
     ######################################################
 
     # generate the radii and thetas that you'll reuse at each timestep
     sample_radii, sample_thetas = generate_sample_radii_thetas(
@@ -881,36 +1067,64 @@
     positions = skypos(**state)
     x_c = positions[0, :]
     y_c = positions[1, :]
     z_c = positions[2, :]
 
     # just the reflected component
     if compute_reflected_phase_curve & (not compute_emitted_phase_curve):
-        reflected = reflected_phase_curve(
-            sample_radii, sample_thetas, two, three, state, x_c, y_c, z_c
-        )
+        if extended_illumination_npts == 1:
+            reflected = reflected_phase_curve(
+                sample_radii, sample_thetas, two, three, state, x_c, y_c, z_c
+            )
+        else:
+            offsets = extended_illumination_offsets(**state)
+            three = planet_3d_coeffs_extended_illumination(**state, offsets=offsets)
+            two = planet_2d_coeffs(**three)
+            reflected = extended_illumination_reflected_phase_curve(
+                sample_radii, sample_thetas, two, three, state, x_c, y_c, z_c, offsets
+            )
         emitted = 0.0
-        # it really didn't make a difference in speed here
-        # reflected = jax.vmap(
-        #     reflected_phase_curve, in_axes=(0, 0, None, None, None, None, None, None)
-        # )(sample_radii, sample_thetas, two, three, state, x_c, y_c, z_c)
-        # reflected = jnp.mean(reflected, axis=0)
 
     # just the emitted component
     elif (not compute_reflected_phase_curve) & compute_emitted_phase_curve:
         reflected = 0.0
         emitted = emission_phase_curve(sample_radii, sample_thetas, two, three, state)
 
     # both reflected and emitted components. this function shares some of the
     # computation between the two, so it's a bit faster than running them separately
-    elif compute_reflected_phase_curve & compute_emitted_phase_curve:
+    elif (
+        compute_reflected_phase_curve
+        & compute_emitted_phase_curve
+        & (extended_illumination_npts == 1)
+    ):
         reflected, emitted = phase_curve(
             sample_radii, sample_thetas, two, three, state, x_c, y_c, z_c
         )
 
+    elif (
+        compute_reflected_phase_curve
+        & compute_emitted_phase_curve
+        & (extended_illumination_npts != 1)
+    ):
+        if extended_illumination_npts == 1:
+            reflected = reflected_phase_curve(
+                sample_radii, sample_thetas, two, three, state, x_c, y_c, z_c
+            )
+        else:
+            offsets = extended_illumination_offsets(**state)
+            three = planet_3d_coeffs_extended_illumination(**state, offsets=offsets)
+            two = planet_2d_coeffs(**three)
+            reflected = extended_illumination_reflected_phase_curve(
+                sample_radii, sample_thetas, two, three, state, x_c, y_c, z_c, offsets
+            )
+        emitted = emission_phase_curve(sample_radii, sample_thetas, two, three, state)
+    else:
+        reflected = 0.0
+        emitted = 0.0
+
     ####################################################
     # compute the star's contribution to the phase curve
     ####################################################
 
     if compute_stellar_ellipsoidal_variations | compute_stellar_doppler_variations:
         time_deltas = state["times"] - state["t_peri"]
         mean_anomalies = 2 * jnp.pi * time_deltas / state["period"]
@@ -926,44 +1140,65 @@
     if compute_stellar_doppler_variations:
         doppler = stellar_doppler_variations(
             true_anomalies, state["stellar_doppler_alpha"], state["period"]
         )
     else:
         doppler = 0.0
 
+    ####################################################
     # put it all together
-    return transit + trend + reflected + emitted + ellipsoidal + doppler
+    ####################################################
+
+    oversampled_curve = transit + trend + reflected + emitted + ellipsoidal + doppler
+    if oversample > 1:
+        c = (oversampled_curve.reshape(-1, oversample) * state["stencil"][None, :]).sum(
+            axis=1
+        )
+    else:
+        c = oversampled_curve
+    return c
 
 
 @partial(
     jax.jit,
     static_argnums=(
         0,
         1,
         2,
         3,
         4,
         5,
+        6,
+        7,
+        8,
     ),
 )
 def _loglike(
     compute_reflected_phase_curve,
     compute_emitted_phase_curve,
     compute_stellar_ellipsoidal_variations,
     compute_stellar_doppler_variations,
+    parameterize_with_projected_ellipse,
+    oversample,
     random_seed,
     phase_curve_nsamples,
+    extended_illumination_npts,
     state,
     params,
 ):
     lc = _lightcurve(
         compute_reflected_phase_curve,
         compute_emitted_phase_curve,
+        compute_stellar_ellipsoidal_variations,
+        compute_stellar_doppler_variations,
+        parameterize_with_projected_ellipse,
+        oversample,
         random_seed,
         phase_curve_nsamples,
+        extended_illumination_npts,
         state,
         params,
     )
 
     for key in params.keys():
         state[key] = params[key]
```

### Comparing `squishyplanet-0.0.1/squishyplanet.egg-info/SOURCES.txt` & `squishyplanet-0.1.0/squishyplanet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.0.1/tests/test_against_jaxoplanet_transit.py` & `squishyplanet-0.1.0/tests/test_against_jaxoplanet_transit.py`

 * *Files identical despite different names*

### Comparing `squishyplanet-0.0.1/tests/test_oblate_system.py` & `squishyplanet-0.1.0/tests/test_oblate_system.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,22 @@
 
         system = OblateSystem(**state)
 
         n = 100_000
         z = system.limb_darkening_profile(jnp.linspace(0, 1, n))
         z *= jnp.linspace(0, 1, n)
 
-        assert jnp.allclose(jnp.trapz(z, jnp.linspace(0, 1, n)) * 2 * jnp.pi, 1.0)
+        # the ui changed for jnp in #20524, don't want to limit versions just for
+        # this though
+        try:
+            val = jnp.trapezoid(z, jnp.linspace(0, 1, n)) * 2 * jnp.pi
+        except:
+            val = jnp.trapz(z, jnp.linspace(0, 1, n)) * 2 * jnp.pi
+
+        assert jnp.allclose(val, 1.0)
 
 
 def test_illustrations():
     state = {
         "t_peri": 0.0,
         "times": jnp.linspace(0.0, 5, 400),
         "a": 2.0,
```

