# Comparing `tmp/PyCESim-0.0.2.tar.gz` & `tmp/PyCESim-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCESim-0.0.2.tar", last modified: Sat Mar 30 18:10:23 2024, max compression
+gzip compressed data, was "PyCESim-0.0.4.tar", last modified: Thu May  2 19:14:09 2024, max compression
```

## Comparing `PyCESim-0.0.2.tar` & `PyCESim-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 fallum   (778712529) 1704612529        0 2024-03-30 18:10:23.059797 PyCESim-0.0.2/
--rw-r--r--   0 fallum   (778712529) 1704612529    35149 2024-03-29 22:05:40.000000 PyCESim-0.0.2/LICENSE
--rw-r--r--   0 fallum   (778712529) 1704612529      389 2024-03-30 18:10:23.059515 PyCESim-0.0.2/PKG-INFO
-drwxr-xr-x   0 fallum   (778712529) 1704612529        0 2024-03-30 18:10:23.056548 PyCESim-0.0.2/PyCESim/
--rw-r--r--   0 fallum   (778712529) 1704612529    27253 2024-03-30 17:24:05.000000 PyCESim-0.0.2/PyCESim/PyCESim.py
--rw-r--r--   0 fallum   (778712529) 1704612529       23 2024-03-30 17:08:58.000000 PyCESim-0.0.2/PyCESim/__init__.py
-drwxr-xr-x   0 fallum   (778712529) 1704612529        0 2024-03-30 18:10:23.059043 PyCESim-0.0.2/PyCESim.egg-info/
--rw-r--r--   0 fallum   (778712529) 1704612529      389 2024-03-30 18:10:23.000000 PyCESim-0.0.2/PyCESim.egg-info/PKG-INFO
--rw-r--r--   0 fallum   (778712529) 1704612529      219 2024-03-30 18:10:23.000000 PyCESim-0.0.2/PyCESim.egg-info/SOURCES.txt
--rw-r--r--   0 fallum   (778712529) 1704612529        1 2024-03-30 18:10:23.000000 PyCESim-0.0.2/PyCESim.egg-info/dependency_links.txt
--rw-r--r--   0 fallum   (778712529) 1704612529       36 2024-03-30 18:10:23.000000 PyCESim-0.0.2/PyCESim.egg-info/requires.txt
--rw-r--r--   0 fallum   (778712529) 1704612529        8 2024-03-30 18:10:23.000000 PyCESim-0.0.2/PyCESim.egg-info/top_level.txt
--rw-r--r--   0 fallum   (778712529) 1704612529       75 2024-03-29 22:05:40.000000 PyCESim-0.0.2/README.md
--rw-r--r--   0 fallum   (778712529) 1704612529       38 2024-03-30 18:10:23.059922 PyCESim-0.0.2/setup.cfg
--rw-r--r--   0 fallum   (778712529) 1704612529      591 2024-03-30 18:07:04.000000 PyCESim-0.0.2/setup.py
+drwxr-xr-x   0 fallum   (778712529) SLAC\Domain Users (1704612529)        0 2024-05-02 19:14:09.460248 PyCESim-0.0.4/
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)    35149 2024-03-29 22:05:40.000000 PyCESim-0.0.4/LICENSE
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)      389 2024-05-02 19:14:09.459978 PyCESim-0.0.4/PKG-INFO
+drwxr-xr-x   0 fallum   (778712529) SLAC\Domain Users (1704612529)        0 2024-05-02 19:14:09.455560 PyCESim-0.0.4/PyCESim/
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)    32243 2024-05-02 18:47:40.000000 PyCESim-0.0.4/PyCESim/PyCESim.py
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)       23 2024-03-30 17:08:58.000000 PyCESim-0.0.4/PyCESim/__init__.py
+drwxr-xr-x   0 fallum   (778712529) SLAC\Domain Users (1704612529)        0 2024-05-02 19:14:09.458767 PyCESim-0.0.4/PyCESim.egg-info/
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)      389 2024-05-02 19:14:09.000000 PyCESim-0.0.4/PyCESim.egg-info/PKG-INFO
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)      219 2024-05-02 19:14:09.000000 PyCESim-0.0.4/PyCESim.egg-info/SOURCES.txt
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)        1 2024-05-02 19:14:09.000000 PyCESim-0.0.4/PyCESim.egg-info/dependency_links.txt
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)       36 2024-05-02 19:14:09.000000 PyCESim-0.0.4/PyCESim.egg-info/requires.txt
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)        8 2024-05-02 19:14:09.000000 PyCESim-0.0.4/PyCESim.egg-info/top_level.txt
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)       96 2024-05-02 18:57:11.000000 PyCESim-0.0.4/README.md
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)       38 2024-05-02 19:14:09.460734 PyCESim-0.0.4/setup.cfg
+-rw-r--r--   0 fallum   (778712529) SLAC\Domain Users (1704612529)      591 2024-05-02 19:13:39.000000 PyCESim-0.0.4/setup.py
```

### Comparing `PyCESim-0.0.2/LICENSE` & `PyCESim-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCESim-0.0.2/PyCESim/PyCESim.py` & `PyCESim-0.0.4/PyCESim/PyCESim.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,23 +22,67 @@
 p_au_KE_eV_fac = (p_au_fac)**2/(u*e) # factor for converting from atomic units of momentum to KE in eV
 cm_to_hartree = 1 / 219474.6 
 hartree_to_eV = 27.211396132
 u_to_amu = 1 / 5.4857990943e-4
 bohr_to_angstrom = 0.529177211
 
 
-atomno_dict = {1:'H',
-               2:'He',
-               3:'Li',
-               4:'Be',
-               5:'B',
-               6:'C',
-               7:'N',
-               8:'O',
-               9:'F'}
+atomno_dict = {'H': 1,
+ 'He': 2,
+ 'Li': 3,
+ 'Be': 4,
+ 'B': 5,
+ 'C': 6,
+ 'N': 7,
+ 'O': 8,
+ 'F': 9,
+ 'Ne': 10,
+ 'Na': 11,
+ 'Mg': 12,
+ 'Al': 13,
+ 'Si': 14,
+ 'P': 15,
+ 'S': 16,
+ 'Cl': 17,
+ 'Ar': 18,
+ 'K': 19,
+ 'Ca': 20,
+ 'Sc': 21,
+ 'Ti': 22,
+ 'V': 23,
+ 'Cr': 24,
+ 'Mn': 25,
+ 'Fe': 26,
+ 'Co': 27,
+ 'Ni': 28,
+ 'Cu': 29,
+ 'Zn': 30,
+ 'Ga': 31,
+ 'Ge': 32,
+ 'As': 33,
+ 'Se': 34,
+ 'Br': 35,
+ 'Kr': 36,
+ 'Rb': 37,
+ 'Sr': 38,
+ 'Y': 39,
+ 'Zr': 40,
+ 'Nb': 41,
+ 'Mo': 42,
+ 'Tc': 43,
+ 'Ru': 44,
+ 'Rh': 45,
+ 'Pd': 46,
+ 'Ag': 47,
+ 'Cd': 48,
+ 'In': 49,
+ 'Sn': 50,
+ 'Sb': 51,
+ 'Te': 52,
+ 'I': 53}
 
 atomcolor_dict = {'H':'snow',
                   'C':'grey',
                   'O':'red',
                   'N':'blue',
                   'F':'yellow',
                   'I':'magenta'}
@@ -98,15 +142,20 @@
           'I': 126.904468}
 
 
 
 # some utility functions
 
 def read_xyz(xyz_file):
-    # Load geometry file as strings
+    """Read in a simple geometry (.xyz) file
+
+    :param xyz_file: .xyz file containing molecular coordinates
+
+    :return: Geometry object"""
+
     with open(xyz_file,'r') as geo_data:
         geo_str = geo_data.readlines()
 
     # Extract element information (elements) and coordinates (geom)
     geo_str_cs = geo_str[2:]
     coordinates = np.zeros((len(geo_str_cs),3))
     element_list = []
@@ -121,71 +170,125 @@
     for element in element_list:
         try:
             mass_list.append(mass_dict[element])
         except KeyError:
             print(f'ERROR: Mass not found for element {element}!')
             
     
-    geom = geometry(coordinates,np.array(mass_list), element_list=element_list)
+    geom = Geometry(coordinates,np.array(mass_list), element_list=element_list)
     return(geom)
 
 
+def read_traj_xyz(xyz_file):
+    """(Experimental) Read in a trajectory (.xyz) file
+
+    :param xyz_file: .xyz file containing series of molecular coordinates, representing different timesteps in a trajectory
+
+    :return:  (list of Geometry objects, list of timesteps)"""
+
+    # Load geometry file as strings
+    with open(xyz_file,'r') as geo_data:
+        geo_str = geo_data.readlines()
+
+    # Extract element information (elements) and coordinates (geom)
+    n_atoms = int(geo_str[0])
+    print(n_atoms)
+
+    geom_list = []
+    time_list = []
+    for time_point in range(0,2000):
+
+        start_line = (time_point)*(n_atoms+2)+2
+        end_line = start_line+n_atoms
+
+        geo_str_cs = geo_str[start_line:end_line]
+        # print(len(geo_str_cs))
+        if len(geo_str_cs):
+            time_string = geo_str[start_line-1].strip()
+            time = float(time_string[7:])
+            coordinates = np.zeros((len(geo_str_cs),3))
+            element_list = []
+            for i in np.arange(len(geo_str_cs)):
+                arr = geo_str_cs[i].split()
+                element_list.append(arr[0])
+                coordinates[i,0] = float(arr[1])
+                coordinates[i,1] = float(arr[2])
+                coordinates[i,2] = float(arr[3])
+            mass_list = []
+            for element in element_list:
+                try:
+                    mass_list.append(mass_dict[element])
+                except KeyError:
+                    print(f'ERROR: Mass not found for element {element}!')
+
+            geom = Geometry(coordinates,np.array(mass_list), element_list=element_list)
+            geom_list.append(geom)
+            time_list.append(time)
+        else:
+            break
+                    
+
+    print('Finished reading at time point %s' % time_point)
+    return(geom_list,time_list)
+
+
+
+
 def read_log(log_file):
+    """Read in a log file. Currently just tested for GAMESS(US)
 
+    :param log_file: '.log' file produced by a quantum chemistry software
+
+    :return: Geometry object
+
+    """
     data = cclib.io.ccread(log_file)
     coordinates = data.atomcoords[-1]
     atomnos = data.atomnos
     atommasses = data.atommasses
     omegas = data.vibfreqs
     nmodes = data.vibdisps
 
-    geom = geometry(coordinates,atommasses,atom_nos=atomnos, omegas=omegas, nmodes=nmodes)
+    geom = Geometry(coordinates,atommasses,atom_nos=atomnos, omegas=omegas, nmodes=nmodes)
     return(geom)
 
 
 
 
 def random_rotation(r_list):
     """
-    Randomly rotate a list of vectors.
+    Randomly rotate a list of vectors. See https://math.stackexchange.com/questions/442418/random-generation-of-rotation-matrices
 
-    Parameters:
-    - r_list: list of vector arrays.
+    :param r_list: list of vector arrays.
 
-    Returns:
-    - r_list_rot: list of rotated vector arrays.
+
+    :return: list of ranomdly rotated vector arrays.
     """
-    
-    ### Random rotation needs an axis and an angle, firstly we generate the vector by randomly selecting on a unit sphere
 
     
-    ### see https://math.stackexchange.com/questions/442418/random-generation-of-rotation-matrices
-    
     r_list_rot = []
-    rm = RandRotationMatrix()
+    rm = rand_rotation_matrix()
     for r in r_list:
         r_list_rot.append(np.dot(rm,r))
     return(r_list_rot)
 
 
-def RandRotationMatrix(deflection=1.0, randnums=None):
+def rand_rotation_matrix(deflection=1.0, randnums=None):
     
-    ### http://blog.lostinmyterminal.com/python/2015/05/12/random-rotation-matrix.html
     """
-    Creates a random rotation matrix.
+    Creates a random rotation matrix. See http://blog.lostinmyterminal.com/python/2015/05/12/random-rotation-matrix.html
+    and http://www.realtimerendering.com/resources/GraphicsGems/gemsiii/rand_rotation.c
 
-    Parameters:
-    - deflection: the magnitude of the rotation. For 0, no rotation; for 1, competely random
+    :param deflection: the magnitude of the rotation. For 0, no rotation; for 1, competely random
     rotation. Small deflection => small perturbation.
-    - randnums: 3 random numbers in the range [0, 1]. If `None`, they will be auto-generated.
+    :param randnums: 3 random numbers in the range [0, 1]. If `None`, they will be auto-generated.
 
-    Returns:
-    - M: random rotation matrix
+    :return: random rotation matrix
+    
     """
-    # from http://www.realtimerendering.com/resources/GraphicsGems/gemsiii/rand_rotation.c
     
     if randnums is None:
         randnums = np.random.uniform(size=(3,))
         
     theta, phi, z = randnums
     
     theta = theta * 2.0*deflection*np.pi  # Rotation about the pole (Z).
@@ -212,46 +315,77 @@
     
     # Construct the rotation matrix  ( V Transpose(V) - I ) R.
     
     M = (np.outer(V, V) - np.eye(3)).dot(R)
     return M
 
 
-def CoulombForce(r1,r2,q1,q2):
-    """Calculate Coulomb force between two charges in SI units."""
+def coulomb_force(r1,r2,q1,q2):
+    """Calculate Coulomb force between two charges in SI units.
+
+    :param r1: (3D) position of charge 1 (in m)
+    :param r2: (3D) position of charge 2 (in m)
+    :param q1: charge 1 (in C)
+    :param q2: charge 2 (in C)
+
+    :return: Coulomb force (in N)"""
+
+
     q1 = q1
     q2 = q2
     r12 = r1-r2
     r12_mag = np.linalg.norm(r12)
     return(k*q1*q2*r12*(1/r12_mag**3))
 
 
 def calc_W(P,Q,n=0):
-    """Calculate unitless Wigner function."""
+    """Calculate unitless Wigner function.
+
+    :param P: unitless momentum
+    :param Q: unitless position
+    :param n: vibrational state (0 by default)
+
+    :return: W(P,Q,n)"""
     if n>0:
         Ln = scipy.special.laguerre(0)
         rhosquare = 2.0 * (P**2 + Q**2)
         Ln = scipy.special.laguerre(n)
         W = (-1.0)**n * Ln(rhosquare) * np.exp(-rhosquare / 2.0)
     else:
         W = np.exp(-Q**2)*np.exp(-P**2)
     return(W)
 
 def calc_canonical_partition(omega, T):
-    """Calculate vibrational canonical partition function."""
+    """Calculate vibrational canonical partition function.
+
+    :param omega: vibrational frequency
+    :param T: temperature (k)
+
+    :return: Z(omega,T) - canonical partition function"""
     Z = np.exp(-(hbar*omega)/(2*kb*T))/(1-np.exp(-(hbar*omega)/(kb*T)))
     return(Z)
 
 def calc_vib_energy(n,omega):
-    """Calculate vibrational energy for given n and frequency."""
+    """Calculate vibrational energy for given n and frequency.
+
+    :param n: vibrational state
+    :param omega: vibrational frequency
+
+    :return: En = hbar * omega * (n+1/2)"""
     En = hbar*omega*(n+1/2)
     return(En)
 
 def calc_Pn(omega_cm, T,n):
-    """Calculate probability of populating vibrational state n."""
+    """Calculate probability of populating vibrational state n.
+
+    :param omega_cm: vibrational frequency (in wavenumbers)
+    :param T: temperature (in K)
+    :param n: vibrational state
+
+    :return: P(n, omega,T) - probability of being in state n"""
     omega_Hz = omega_cm*c_cm_s*2*np.pi
     Z = calc_canonical_partition(omega_Hz,T)
     En = calc_vib_energy(n, omega_Hz)
     if T>0:
         Pn = np.exp(-En/(kb*T))/Z
     # probably don't need this to deal with T=0 but no harm
     else:
@@ -259,16 +393,26 @@
             Pn = 1
         else:
             Pn = 0
     return(Pn)
 
 
 
-class geometry:
-    """Class for (equilibrium) molecular geometry and related information."""
+class Geometry:
+    """Class for (equilibrium) molecular geometry and related information.
+
+    :param atom_coords: numpy array of the 3D position of each atom in the structure
+    :param atom_masses: numpy array of the atomic mass of each atom in the structure
+    :param element_list: list of element of each atom
+    :param atom_nos: list of atomic numbers of each atom
+    :param atom_labels: list of strings used to label each atom
+    :param geom_label: Optional, additional label used to identify this geometry
+    :param nmodes: Optional, normal modes
+    :param omegs: Optional, vibrational frequencies
+    """
     def __init__(self, atom_coords, atom_masses, element_list=[], atom_nos = np.array([]), 
                  atom_labels = np.array([]), geom_label=None, nmodes=np.array([]), omegas=np.array([])):
         self.atom_coords = np.array(atom_coords)
         self.atom_masses = np.array(atom_masses)
         self.natoms = len(atom_coords)
         if atom_nos.any():
             self.atom_nos = atom_nos
@@ -282,24 +426,31 @@
         if nmodes.any():
             self.nmodes = nmodes
             self.check_normal_modes()
         if omegas.any():
             self.omegas = omegas
             
     def get_elements(self):
-        """Gets elements from atomic numbers"""
+        """Gets list of elements (stored in self.element_list) from atomic numbers (stored in self.atom_nos)"""
         element_list = []
         for atomno in self.atom_nos:
             if atomno in atomno_dict:
                 element_list.append(atomno_dict[atomno])
             else:
                 element_list.append('?')
         self.element_list = element_list
 
     def visualize_2D(self, dim1=0, dim2=1, markersize=30, markeredgewidth=3):
+        """Visualizes a 2D projection of the molecular structure
+
+        :param dim1: first dimension (0=x, 1=y etc.) of the 2D histogram
+        :param dim2: second dimension (0=x, 1=y etc.) of the 2D histogram
+        :param markersize: size of atom marker (default 30)
+        :param markeredgewidth: edgewidth of atom marker (default 3)
+        """
         dim_list=['x','y','z']
         dim1_range = (np.min(self.atom_coords[:,dim1])-0.5, np.max(self.atom_coords[:,dim1])+0.5)
         dim2_range = (np.min(self.atom_coords[:,dim2])-0.5, np.max(self.atom_coords[:,dim2])+0.5)
 
         fig,ax=plt.subplots(figsize=(4,4))
         ax.set_xlim(dim1_range[0],dim1_range[1])
         ax.set_ylim(dim2_range[0],dim2_range[1])
@@ -312,30 +463,31 @@
             ax.plot(coord[dim1], coord[dim2], 'o', color=color, markersize=markersize, 
                 markeredgewidth=markeredgewidth, markeredgecolor='black')
         ax.set_xlabel(dim_list[dim1] + r" / $\mathrm{\AA}$ ", fontsize=14)
         ax.set_ylabel(dim_list[dim2] + r" / $\mathrm{\AA}$ ", fontsize=14)
         plt.show()
 
     def find_com(self):
-        """Find centre-of-mass of geometry."""
+        """Find centre-of-mass of geometry. Stored in self.com"""
         mass_product = np.zeros((3,))
         mass_sum = 0
         for r, mass in zip(self.atom_coords,self.atom_masses):
             mass_product+=r*mass
             mass_sum+=mass
         self.com = mass_product/mass_sum
 
     def com_geometry(self):
-        """Shift geometry to set centre-of-mass to zero."""
+        """Shift geometry to set centre-of-mass to zero.
+        New geometry is stored in self.atom_coods_com"""
         self.find_com()
         self.atom_coords_com = self.atom_coords - self.com
 
 
     def check_normal_modes(self, threshold=0.05, make_fig=True):
-        """Check if normal modes are orthogonal re-weight them correctly.
+        """Check if normal modes are orthogonal and re-weight them correctly (in self.nmodes_weighted).
         Currently function works for GAMESS format modes, need to expand to other formats."""
     
         results = np.zeros((len(self.nmodes),len(self.nmodes)))
         nmodes2 = []
         
         for mode in self.nmodes:
             norm=0
@@ -379,32 +531,40 @@
         if np.max(abs(results))>threshold:
             print('Normal modes are NOT in expected format')
         else:
             print('Normal modes are in expected format')
         self.nmodes_weighted = nmodes2
 
 
-class ce_channel:
+class CEChannel:
     """Class for CE channel. For now this refers to a charge distribution, but could be extended
-    to capture different (molecular) fragments etc."""
+    to capture different (molecular) fragments etc.
+
+    :param charges: array of charges
+    :param p: probability of this channel occuring in the simulation"""
     def __init__(self, charges, p, label='None'):
         self.charges = np.array(charges)
         self.p = p
         if label:
             self.label=label
 
 
-class starting_conditions:
-    """Class for generating starting conditions for CE simulation."""
+class StartingConditions:
+    """Class for generating starting conditions for CE simulation.
+
+    :param eq_geometry: (equilibrium) geometry"""
     
     def __init__(self, eq_geometry):
         self.eq_geometry = eq_geometry
         self.multi_channel=False
 
     def set_channel_list(self, channel_list):
+        """Add a list of different channels to the object
+
+        :param channel_list: list of CEChannel objects"""
         channel_p_list = []
         for channel in channel_list:
             channel_p_list.append(channel.p)
         sum_p = np.sum(channel_p_list)
         if abs(sum_p-1)>0.01:
             print(f"Channel probabilities sum to {sum_p}. Will rescale anyway.")
         else:
@@ -421,24 +581,25 @@
         # First check if sigma is a single number, convert to single number array if so
         if isinstance(self.sigma, (int, float, complex)) and not isinstance(self.sigma, bool):
             self.sigma = np.array([self.sigma])
             
 
     def generate_pool(self, n_geoms, method='gaussian',random_rotate=True, sigma=0.1, wigner_sample_max=3, T=0, nmax=5):
         """Main method for generating the pool of starting conditions for simulation.
-        Parameters:
-        - n_geoms: number of samples in the pool
-        method: ['gaussian', 'wigner'] method of blurring geometries. If 'gaussian', geometries are just convolved
+
+        :param n_geoms: number of samples in the pool
+        :param method: ['gaussian', 'wigner'] method of blurring geometries. If 'gaussian', geometries are just convolved
         by a Gaussian distribution of width sigma. If 'wigner', instead sample from vibrational wigner distribution
         with a specified temeprature. This requires the geometry to include normal modes as appropriate.
-        sigma: sigma for Gaussian convolution
-        random_rotate: if True, randomly rotate each sampled geometry
-        wigner_sample_max: the max (absolute) value of P and Q used for Wigner sampling
-        T: temperature for wigner sampling
-        nmax: max vibrational state considered for wigner sampling
+        :param sigma: sigma for Gaussian convolution
+        :param random_rotate: if True, randomly rotate each sampled geometry
+        :param wigner_sample_max: the max (absolute) value of P and Q used for Wigner sampling
+        :param T: temperature for wigner sampling
+        :param nmax: max vibrational state considered for wigner sampling
+
         """
         self.method = method
         if self.method=='wigner':
             # If generating a pool of simulations by Wigner sampling, we need
             # the normal modes, their frequencies, and a temperature
             assert self.eq_geometry.nmodes.any()
             assert self.eq_geometry.omegas.any()
@@ -550,14 +711,21 @@
                 y0[3*n+2] = (r_list_rot[n][2])
                 
             self.samp_y0_list.append(y0)
             self.samp_charges_list.append(charges)
             self.samp_masses_list.append(masses)
 
     def visualize_pool_2D(self, dim1=0,dim2=1, vmax=100, nbins=200):
+        """Function for visualizing the 2D pool of geometries as a 2D histogram.
+
+        :param dim1: First dimension (0=x, 1=y etc.) of histogram. Default 0
+        :param dim2: Second dimension (0=x, 1=y etc.) of histogram. Default 1
+        :param vmax: Maximum for colorbar. Default 100
+        :param nbins: Number of bins in each dimension for 2D histogram. Default 200
+        """
         dim_list=['x','y','z']
         vis_geom_list = []
         for y0 in self.samp_y0_list:
             for n in range(self.eq_geometry.natoms):
                 vis_geom_list.append(y0[n*3:n*3+3]*1e10)
 
         vis_geom_arr =np.vstack(vis_geom_list)
@@ -573,55 +741,56 @@
         ax.set_xlim(dim1_range[0],dim1_range[1])
         ax.set_ylim(dim2_range[0],dim2_range[1])
         ax.set_xlabel(dim_list[dim1] + r" / $\mathrm{\AA}$ ", fontsize=14)
         ax.set_ylabel(dim_list[dim2] + r" / $\mathrm{\AA}$ ", fontsize=14)
         plt.show()
 
     def wigner_histograms(self):
+        """Quick plot of histograms of n and Q"""
         fig,ax=plt.subplots(figsize=(4,3))
         ax.hist(self.samp_n_list, bins=np.arange(self.nmax)-0.5)
         ax.set_xlabel(r'n$_{\mathrm{vib}}$', fontsize=14)
         ax.set_ylabel('no.', fontsize=14)
         plt.show()
 
         fig,ax=plt.subplots(figsize=(4,3))
         ax.hist(self.samp_q_list, range=(-self.wigner_sample_max,self.wigner_sample_max), bins=int(self.n_geoms/20))
         ax.set_xlabel('Q', fontsize=14)
         ax.set_ylabel('no.', fontsize=14)
         plt.show()
             
-class CE_sim:
-    """Class for CE simulation results and methods."""
+class CESim:
+    """Class for CE simulation results and methods.
+    :param starting_conditions:"""
     def __init__(self, starting_conditions):
         self.starting_conditions=starting_conditions
 
     def make_timebins(self, t_range_list, n_step_list):
         """Create timebins for simulation.
         
-        Parameters:
-        - t_range_list: list of tuples of (t1,t2) between which we will populate timestemps
-        - n_step_list: number of timestemps to be populated within each range (t1,t2)
+        :param t_range_list: list of tuples of (t1,t2) between which we will populate timestemps
+        :param n_step_list: number of timestemps to be populated within each range (t1,t2)
         """
         tsteps_list = []
         for t_range, n_step in zip(t_range_list,n_step_list):
             t_steps = np.linspace(t_range[0],t_range[1], n_step)
             tsteps_list.append(t_steps)
 
         tsteps_full = np.concatenate(tsteps_list)
         self.set_timebins(tsteps_full)
         
     def set_timebins(self, timebins):
-        """Store timebins for simulation."""
+        """Store timebins and related parameters for simulation."""
         self.timebins=timebins
         self.tmin = np.min(timebins)
         self.tmax = np.max(timebins)
         self.n_t_steps = len(self.timebins)
 
     def store_output(self, solution):
-        """Take solution from ODE solver and convert to output."""
+        """Take solution from ODE solver and convert to output (stored in self.output_list)."""
         charges = self.starting_conditions.samp_charges_list[self.sim_counter]
         masses = self.starting_conditions.samp_masses_list[self.sim_counter]
         
 
         n_atoms = len(charges)
         
         output_array = np.zeros((n_atoms,7))
@@ -638,19 +807,21 @@
             else:
                 output_array[i,5]=0
             output_array[i,6] = self.sim_counter
 
         self.output_list.append(output_array)
 
     def output_list_to_arr(self):
-        """Convert simulation output from list of arrays to a single array"""
+        """Convert simulation output from list of arrays (self.output_list) 
+        to a single array (self.output_arr)"""
         self.output_arr = np.vstack(self.output_list)
 
     def output_list_to_df(self):
-        """Convert simulation output from list of arrays to a Pandas dataframe"""
+        """Convert simulation output from list of arrays to a Pandas dataframe
+        (stored in self.output_df)"""
         try:
             self.output_df = pd.DataFrame(self.output_arr, columns = ['vx_ms','vy_ms','vz_ms','charge_C','mass_kg', 'channel_idx', 'sim_counter'])
         except:
             self.output_list_to_arr()
             self.output_df = pd.DataFrame(self.output_arr, columns = ['vx_ms','vy_ms','vz_ms','charge_C','mass_kg', 'channel_idx', 'sim_counter'])
 
         self.output_df['charge_e'] = self.output_df['charge_C']/e
@@ -673,38 +844,36 @@
         """Simulate CE for each starting condition"""
         self.output_list=[]
         self.save_all=save_all
         if self.save_all:
             self.solution_list = []
         self.sim_counter=0
         for y0 in self.starting_conditions.samp_y0_list:
-            solution = solve_ivp(self.NewtonEquations, [0, self.tmax], y0, t_eval = self.timebins)
+            solution = solve_ivp(self.newton_equations, [0, self.tmax], y0, t_eval = self.timebins)
             if save_all:
                 self.solution_list.append(solution)
             self.store_output(solution)
             if self.sim_counter%n_print==0:
                 print(f'On simultion number {self.sim_counter}!')
             self.sim_counter+=1
         if make_df:
             self.output_list_to_df()
 
 
 
-    def NewtonEquations(self,t,y):
+    def newton_equations(self,t,y):
         """Setup Newton equations for ODE solver.
 
-        Parameters:
-        - t = array of timebins for ODE calculation.
-        - y = the first natoms*3 elements are x,y,z positions of each atom. 
+        :param t: array of timebins for ODE calculation.
+        :param y: the first natoms*3 elements are x,y,z positions of each atom. 
         The next natoms*3 elements are vx,vy,vz of each atom
 
-        Returns:
-
-        -dydt: the first natoms*3 are vx,vy,vz positions of each atom (i.e second half of y). 
+        :return: dydt array the first natoms*3 are vx,vy,vz positions of each atom (i.e second half of y). 
         Next natoms*3 are ax,ay,az (from F=ma)
+
         """
 
         charges = self.starting_conditions.samp_charges_list[self.sim_counter]
         masses = self.starting_conditions.samp_masses_list[self.sim_counter]
         
         dydt = np.zeros((np.shape(y)))
         n_atoms = np.shape(y)[0]/6
@@ -717,15 +886,15 @@
             
             ## Now calculate forces
             force = np.zeros((3,))
             for k in range(n_atoms):
                 if k!=n:
                     r1 = np.array([y[3*n], y[3*n+1], y[3*n+2]])
                     r2 = np.array([y[3*k], y[3*k+1], y[3*k+2]])
-                    force += CoulombForce(r1,r2, charges[n], charges[k])
+                    force += coulomb_force(r1,r2, charges[n], charges[k])
                 
             dydt[3*n_atoms+3*n:3*n_atoms+3*n+3] = force/masses[n]
     
         return(dydt)
```

### Comparing `PyCESim-0.0.2/setup.py` & `PyCESim-0.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'PyCESim - classical simulation of Coulomb explosion'
 
 setup(
         name="PyCESim", 
         version=VERSION,
         author="Felix Allum",
         author_email="fallum@stanford.edu",
         description=DESCRIPTION,
         packages=find_packages(),
         install_requires=['cclib', 'numpy', 'matplotlib', 'scipy', 'pandas'],
         url='https://github.com/f-allum/PyCESim/',
-        download_url='https://github.com/f-allum/PyCESim/archive/refs/tags/v0.0.2.tar.gz',
+        download_url='https://github.com/f-allum/PyCESim/archive/refs/tags/v0.0.3.tar.gz',
         keywords=['Coulomb explosion']
 )
```

