# Comparing `tmp/snorer-1.0.0.tar.gz` & `tmp/snorer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snorer-1.0.0.tar", last modified: Wed May  1 05:49:51 2024, max compression
+gzip compressed data, was "snorer-1.0.1.tar", last modified: Thu May  2 14:01:02 2024, max compression
```

## Comparing `snorer-1.0.0.tar` & `snorer-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-05-01 05:49:51.632844 snorer-1.0.0/
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    35129 2024-03-29 01:27:08.000000 snorer-1.0.0/LICENSE
--rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    49151 2024-05-01 05:49:51.632844 snorer-1.0.0/PKG-INFO
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     8123 2024-05-01 05:46:42.000000 snorer-1.0.0/README.md
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1094 2024-05-01 05:49:34.000000 snorer-1.0.0/pyproject.toml
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       38 2024-05-01 05:49:51.632844 snorer-1.0.0/setup.cfg
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       49 2024-03-28 13:38:04.000000 snorer-1.0.0/setup.py
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-05-01 05:49:51.628844 snorer-1.0.0/src/
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-05-01 05:49:51.632844 snorer-1.0.0/src/snorer/
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1983 2024-05-01 05:49:34.000000 snorer-1.0.0/src/snorer/__init__.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     4299 2024-04-29 15:04:44.000000 snorer-1.0.0/src/snorer/constants.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     9088 2024-04-27 15:23:37.000000 snorer-1.0.0/src/snorer/geometry.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    18337 2024-04-30 11:09:15.000000 snorer-1.0.0/src/snorer/halo.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    14000 2024-05-01 02:58:10.000000 snorer-1.0.0/src/snorer/kinematics.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    13472 2024-04-30 11:21:06.000000 snorer-1.0.0/src/snorer/snorerMain.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1230 2024-04-28 14:34:31.000000 snorer-1.0.0/src/snorer/sysmsg.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    17991 2024-05-01 02:58:17.000000 snorer-1.0.0/src/snorer/utils.py
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-05-01 05:49:51.632844 snorer-1.0.0/src/snorer.egg-info/
--rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    49151 2024-05-01 05:49:51.000000 snorer-1.0.0/src/snorer.egg-info/PKG-INFO
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      390 2024-05-01 05:49:51.000000 snorer-1.0.0/src/snorer.egg-info/SOURCES.txt
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        1 2024-05-01 05:49:51.000000 snorer-1.0.0/src/snorer.egg-info/dependency_links.txt
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       56 2024-05-01 05:49:51.000000 snorer-1.0.0/src/snorer.egg-info/requires.txt
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        7 2024-05-01 05:49:51.000000 snorer-1.0.0/src/snorer.egg-info/top_level.txt
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-05-02 14:01:02.732234 snorer-1.0.1/
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    35129 2024-03-29 01:27:08.000000 snorer-1.0.1/LICENSE
+-rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    49586 2024-05-02 14:01:02.732234 snorer-1.0.1/PKG-INFO
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     8558 2024-05-01 11:53:30.000000 snorer-1.0.1/README.md
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1094 2024-05-02 14:00:20.000000 snorer-1.0.1/pyproject.toml
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       38 2024-05-02 14:01:02.732234 snorer-1.0.1/setup.cfg
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       49 2024-03-28 13:38:04.000000 snorer-1.0.1/setup.py
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-05-02 14:01:02.724234 snorer-1.0.1/src/
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-05-02 14:01:02.732234 snorer-1.0.1/src/snorer/
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1983 2024-05-02 14:00:20.000000 snorer-1.0.1/src/snorer/__init__.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     4299 2024-05-02 02:21:28.000000 snorer-1.0.1/src/snorer/constants.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     9088 2024-04-27 15:23:37.000000 snorer-1.0.1/src/snorer/geometry.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    18337 2024-04-30 11:09:15.000000 snorer-1.0.1/src/snorer/halo.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    14603 2024-05-02 13:18:34.000000 snorer-1.0.1/src/snorer/kinematics.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    13472 2024-04-30 11:21:06.000000 snorer-1.0.1/src/snorer/snorerMain.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1230 2024-04-28 14:34:31.000000 snorer-1.0.1/src/snorer/sysmsg.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    17982 2024-05-02 02:20:21.000000 snorer-1.0.1/src/snorer/utils.py
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-05-02 14:01:02.732234 snorer-1.0.1/src/snorer.egg-info/
+-rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    49586 2024-05-02 14:01:02.000000 snorer-1.0.1/src/snorer.egg-info/PKG-INFO
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      390 2024-05-02 14:01:02.000000 snorer-1.0.1/src/snorer.egg-info/SOURCES.txt
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        1 2024-05-02 14:01:02.000000 snorer-1.0.1/src/snorer.egg-info/dependency_links.txt
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       56 2024-05-02 14:01:02.000000 snorer-1.0.1/src/snorer.egg-info/requires.txt
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        7 2024-05-02 14:01:02.000000 snorer-1.0.1/src/snorer.egg-info/top_level.txt
```

### Comparing `snorer-1.0.0/LICENSE` & `snorer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snorer-1.0.0/PKG-INFO` & `snorer-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snorer
-Version: 1.0.0
+Version: 1.0.1
 Summary: This package evaluates the time-of-flight signatures of boosted dark matter due to supernova neutrinos from our Milky Way
 Author-email: Yen-Hsun Lin <yenhsun@phys.ncku.edu.tw>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -691,31 +691,40 @@
 <a href = "https://choosealicense.com/licenses/gpl-3.0/"  target = "_blank">![License](https://img.shields.io/badge/License-GPL_3.0-blue.svg)</a>
 <a href = "https://arxiv.org/abs/2206.06864"  target = "_blank">![ArXiv](https://img.shields.io/badge/arXiv-2206.06864-yellowgreen.svg)</a>
 <a href = "https://arxiv.org/abs/2307.03522"  target = "_blank">![ArXiv](https://img.shields.io/badge/arXiv-2307.03522-yellowgreen.svg)</a>
 
 # snorer: *S*upernova-*N*eutrino-b*O*osted da*R*k matt*ER*
 
 
-`snorer` is a package for evaluating time-of-flight signatures of supernova-neutrino-boosted dark matter (SN*ν* BDM) from our Milky Way (MW) and SN1987a in Large Magellanic Cloud (LMC) based on
+`snorer` is a package for evaluating time-of-flight signatures of supernova-neutrino-boosted dark matter (SN*ν* BDM) from our Milky Way (MW), SN1987a in Large Magellanic Cloud (LMC) and SN in arbitrary distant galaxy based on
 <a href = "https://doi.org/10.1103/PhysRevLett.130.111002" target = "_blank">*Phys. Rev. Lett.* **130**, 111002 (2023)</a> [<a href = "https://arxiv.org/abs/2206.06864" target = "_blank">arXiv:2206.06864</a>]
 and
 <a href = "https://doi.org/10.1103/PhysRevD.108.083013" target = "_blank">*Phys. Rev. D* **108**, 083013 (2023)</a>
 [<a href = "https://arxiv.org/abs/2307.03522" target = "_blank">arXiv:2307.03522</a>].
 
+### Citation
+
+If you use this package or part of the code in your research, please cite the followings:
+
+1. Y.-H. Lin *et al.*, *Phys. Rev. Lett.* **130**, 111002 (2023), arXiv:2206.06864
+2. Y.-H. Lin *et al.*, *Phys. Rev. D* **108**, 083013 (2023), arXiv:2307.03522
+3. `snorer`: https://github.com/yenhsunlin/snorer
+
+
 ## Installation
 
 To install, excute the following command on the prompt
 
     $ pip install snorer
 
 and everything should be processed on-the-fly.
 
 ### Dependency
 
-`snorer` requires python >= 3.8 and the following packages these external packages
+`snorer` requires python >= 3.8 and the following external packages
 
 - `numpy` >= 1.20.0
 - `scipy` >= 1.10.0
 - `vegas` >= 6.0.1
 - `astropy` >= 6.0.0
 
 where `vegas` is a the backend engine for evaluating multidimensional integrals based on adaptive Monte Carlo vegas algorithm, see its homepage: <a heref = "https://pypi.org/project/vegas/" target = "_blank">https://pypi.org/project/vegas/</a>.
@@ -728,22 +737,22 @@
 We briefly summarize the usage in this section and a comprehensive tutorial can be found in the jupyter notebook in `examples/tutorial.ipynb`.
 
 To import, do
 
     >>> import snorer
 
 in python terminal and is similar in the jupyter notebook.
-All functions and classes can be accessed by typing `snorer.foo()` where `foo` is the name.
+All functions and classes can be accessed by typing `snorer.foo()` where `foo` is the function/class/module name.
 
 
 
 
 ### Useful Constants
 
-We document various useful physical constants and conversion factors...etc as the *attributes* of an instance `snorer.constant`.
+We document various useful physical constants and conversion factors...etc as the *attributes* of the instance `snorer.constant`.
 For example, we can retrieve
 
     >>> snorer.constant.me      # electron mas, MeV
     0.511
     >>> snorer.constant.kpc2cm  # kpc to cm
     3.085e+21
 
@@ -763,90 +772,92 @@
     >>> Tx,mx = 15,0.075
     >>> snorer.get_vx(Tx,mx)
     0.9999876239921284
 
 
 ### SN*ν* BDM Flux 
 
-The BDM flux, or *afterglow* to the ${\rm SN}\nu$, due to SN that is $R_\star$ distant away from us can be evaluated by 
+The BDM flux, or *afterglow* to the ${\rm SN}\nu$, due to SN exploded at $R_\star$ distant away from us can be evaluated by 
 
 $$
 \frac{d\Phi_{\chi}(T_\chi, t^\prime)}{dT_{\chi}dt} =
 \tau\int_0^{2\pi} d\phi\int_{0}^{\pi/2}\sin\theta d\theta~ \mathcal{J} j_{\chi}(r(\phi),D,T_{\chi},\psi)
 $$
 
 where $t$ is the BDM ToF with time-zero at the discovery of SN*ν* on Earth and $t^\prime$ is the total time. We focus on $t$ instead of $t^\prime$.
 Zenith angle $\theta$ and azimuthal angle $\phi$ are relative to the SN-Earth line-of-sight. The default DM-*ν* cross section is $\sigma_{\chi\nu}=10^{-45}$ cm<sup>2</sup>.
 
-The function to evaluate this flux is `snorer.flux()` with $(t,T_\chi,m_\chi,R_\star,\beta)$ are the necessary inputs. 
-Suppose SN's location is at GC, we have $R_\star=8.5$ kpc and $\beta=0$, and examine the flux with turning on DM spike feature
+The function to evaluate this is `snorer.flux()` with $(t,T_\chi,m_\chi,R_\star,\beta)$ are the necessary inputs. 
+Suppose SN's location is at GC, we have $R_\star=8.5$ kpc and $\beta=0$, with default GC-Earth distance $R_e=8.5$ kpc, too.
+With DM spike included, the BDM flux can be calcualted
 
     >>> t,Tx,mx,Rstar,beta = 100,15,1e-2,8.5,0
-    >>> snorer.flux(t,Tx,mx,Rstar,beta,neval=15000)
+    >>> snorer.flux(t,Tx,mx,Rstar,beta,is_spike=True,neval=15000)
     4.572295175982701e-16
 
-Users can turn off the spike feature by inserting `is_spike=False` and will find both numerical results are similar. It implies the contribution to the BDM flux is due to the place outside the spike's influencial region.
+Users can of course turn off the spike feature by setting `is_spike=False` and will find both numerical results are similar.
+It implies the contribution to the BDM flux comes from the place outside the spike's influence.
 
 ### SN*ν* BDM Event
 
 The BDM event number in a detector after exposing to the flux for a period of time, $(t_{\rm min},t_{\rm max})$, can be evaluated by
 
 $$
 N_{\rm BDM} = \int_{t_{\rm min}}^{\rm t_{\rm max}} dt \int_{T_{\chi,{\rm min}}}^{T_{\chi,{\rm max}}}
 \frac{d\Phi_{\chi}(T_\chi, t^\prime)}{dT_{\chi}dt} \times N_e \sigma_{\chi e}
 $$
 
 where $N_e$ is the total electron number in the detector and $\sigma_{\chi e}$ the DM-*e* cross section.
-This can be accomplished by `snorer.event()` with $(m_\chi,R_\star,\beta)$ the necessary inputs.
+This task can be accomplished by `snorer.event()` with $(m_\chi,R_\star,\beta)$ the necessary inputs.
 The default $(t_{\rm min},t_{\rm max})=(10~{\rm s},35~{\rm yrs})$ and $(T_{\chi,{\rm min}},T_{\chi,{\rm max}})=(5,30)$ MeV.
 
 Note that this function is normalized to $N_e=1$ and $\sigma_{\chi e}=1$ cm<sup>2</sup>.
 To have the correct $N_{\rm BDM}$ in a specific detector, users have to mutiply the corresponding $N_e$ and $\sigma_{\chi e}$.
 
 Now let $m_\chi=0.015$ MeV,
 
     >>> mx,Rstar,beta = 0.015,8,0
     >>> N_BDM = snorer.event(mx,Rstar,beta,is_spike=False,neval=50000)
     >>> N_BDM
     1.662174035857532e-06
 
-Suppose it happened in Super-Kamiokande with $N_e\approx 7\times 10^{33}$ and assume $\sigma_{\chi e}=10^{-30}$ cm<sup>2</sup>. The correct $N_{\rm BDM}$ would be
+For Super-Kamiokande, it has $N_e\approx 7\times 10^{33}$ and assume $\sigma_{\chi e}=10^{-35}$ cm<sup>2</sup>. The associated $N_{\rm BDM}$ is
 
     >>> Ne,sigma_xe = 7e33,1e-35
     >>> N_BDM*Ne*sigma_xe
     1.1635218251002724e-07
 
 ### *Experimental* :: Implementation of Particle Physics Model and SN in Arbitrary Distant Galaxy
 
-The aforementioned functions for evaluating BDM signatures are based on model-agnostic picture. It means the cross sections between dark and visble sectors are generally independent of any physical quantities, eg. energy, mass and coupling constants.
+The aforementioned functions for evaluating BDM signatures are based on model-agnostic picture. It means the cross sections between dark and visble sectors are generally independent of physical quantities, eg. energy, mass and coupling constants.
 
-The most important feature of `snorer` is that it offers a general interface for users to implement their favorite particle models.
-Furthermore, SN is not necessary residing in MW or LMC. As long as users can provide these celetial objects' coordinates expressed in *ICRS J2000.0* system, `snorer` can do the calculation.
+The most important feature `snorer` carries is that it offers a general interface for users to implement their favorite particle models.
+Furthermore, SN is not necessary exploding in our MW or LMC. As long as users can provide these celetial objects' coordinates and expressed them in *ICRS J2000.0* metrics, `snorer` can do the calculation.
 `snorer` also allows users to customize the halo shape, by manipulating $\rho_s$, $r_s$ and $n$...etc, and including or excluding spike feature, of such distant galaxy.
 
-This will be done by introducing a *class* `snorer.GeneralInterface`.
-All these user-specified features will compose an instance of `snorer.GeneralInterface`.
+This will be done by the *class* `snorer.GeneralInterface`.
+All these user-specified features will be composed into an instance of `snorer.GeneralInterface`.
 The BDM signatures can be evaluated by calling the associated *methods* within it.
 We have an example in `examples/tutorial.ipynb`, also see the in-class docstring for more information.
 
 
-### Other Useful Functions Classes
+### Other Useful Functions and Classes
 
 We also provide many useful functions and classes at users' disposal. See `examples/tutorial.ipynb` for details.
 
 ## Known Issue
 
 To evaluate BDM event, `snorer` uses `vegas` to handle the multidimensional integration.
-The sampling method of `vegas` cannot manipulate`snorer.event()` as well as the method in the instance of `snorer.GeneralInterface` properly, when SN is exactly at GC with spike feature turning on and no DM self-annihilation.
+The sampling method of `vegas` cannot manipulate event calculation, e.g. `snorer.event()` and the method in the instance of `snorer.GeneralInterface`, properly, when SN is exactly at GC with spike and no DM self-annihilation.
 
 Since the spike is a highly singular behavior, the sampling method may miss the substantial DM contribution from the inner galactic region and causes underestimate of $N_{\rm BDM}$ plus unstable results. 
-To avoid this, users may try to displace the SN from GC when evaluating $N_{\rm BDM}$ whith DM sipke turning on and no DM annihilation.
+To avoid this, users may try to displace the SN from GC a little bit when evaluating $N_{\rm BDM}$ with DM sipke and no DM annihilation.
 For BDM flux evaluation, there is no such issue.
 
 To be fair, the probability of a very cuspy DM spike surving the gravitational disturbance without annihilating away and SN happening exactly at the GC might be very rare.
 
-This issue is scheduled to fix in the next version of `snorer`.
+This issue is scheduled to fix in the next major update of `snorer`.
 
 ## Bugs and troubleshooting
 
 Please report to the author, Yen-Hsun Lin, via [yenhsun@phys.ncku.edu.tw](mailto:yenhsun@phys.ncku.edu.tw).
```

### Comparing `snorer-1.0.0/README.md` & `snorer-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,31 +2,40 @@
 <a href = "https://choosealicense.com/licenses/gpl-3.0/"  target = "_blank">![License](https://img.shields.io/badge/License-GPL_3.0-blue.svg)</a>
 <a href = "https://arxiv.org/abs/2206.06864"  target = "_blank">![ArXiv](https://img.shields.io/badge/arXiv-2206.06864-yellowgreen.svg)</a>
 <a href = "https://arxiv.org/abs/2307.03522"  target = "_blank">![ArXiv](https://img.shields.io/badge/arXiv-2307.03522-yellowgreen.svg)</a>
 
 # snorer: *S*upernova-*N*eutrino-b*O*osted da*R*k matt*ER*
 
 
-`snorer` is a package for evaluating time-of-flight signatures of supernova-neutrino-boosted dark matter (SN*ν* BDM) from our Milky Way (MW) and SN1987a in Large Magellanic Cloud (LMC) based on
+`snorer` is a package for evaluating time-of-flight signatures of supernova-neutrino-boosted dark matter (SN*ν* BDM) from our Milky Way (MW), SN1987a in Large Magellanic Cloud (LMC) and SN in arbitrary distant galaxy based on
 <a href = "https://doi.org/10.1103/PhysRevLett.130.111002" target = "_blank">*Phys. Rev. Lett.* **130**, 111002 (2023)</a> [<a href = "https://arxiv.org/abs/2206.06864" target = "_blank">arXiv:2206.06864</a>]
 and
 <a href = "https://doi.org/10.1103/PhysRevD.108.083013" target = "_blank">*Phys. Rev. D* **108**, 083013 (2023)</a>
 [<a href = "https://arxiv.org/abs/2307.03522" target = "_blank">arXiv:2307.03522</a>].
 
+### Citation
+
+If you use this package or part of the code in your research, please cite the followings:
+
+1. Y.-H. Lin *et al.*, *Phys. Rev. Lett.* **130**, 111002 (2023), arXiv:2206.06864
+2. Y.-H. Lin *et al.*, *Phys. Rev. D* **108**, 083013 (2023), arXiv:2307.03522
+3. `snorer`: https://github.com/yenhsunlin/snorer
+
+
 ## Installation
 
 To install, excute the following command on the prompt
 
     $ pip install snorer
 
 and everything should be processed on-the-fly.
 
 ### Dependency
 
-`snorer` requires python >= 3.8 and the following packages these external packages
+`snorer` requires python >= 3.8 and the following external packages
 
 - `numpy` >= 1.20.0
 - `scipy` >= 1.10.0
 - `vegas` >= 6.0.1
 - `astropy` >= 6.0.0
 
 where `vegas` is a the backend engine for evaluating multidimensional integrals based on adaptive Monte Carlo vegas algorithm, see its homepage: <a heref = "https://pypi.org/project/vegas/" target = "_blank">https://pypi.org/project/vegas/</a>.
@@ -39,22 +48,22 @@
 We briefly summarize the usage in this section and a comprehensive tutorial can be found in the jupyter notebook in `examples/tutorial.ipynb`.
 
 To import, do
 
     >>> import snorer
 
 in python terminal and is similar in the jupyter notebook.
-All functions and classes can be accessed by typing `snorer.foo()` where `foo` is the name.
+All functions and classes can be accessed by typing `snorer.foo()` where `foo` is the function/class/module name.
 
 
 
 
 ### Useful Constants
 
-We document various useful physical constants and conversion factors...etc as the *attributes* of an instance `snorer.constant`.
+We document various useful physical constants and conversion factors...etc as the *attributes* of the instance `snorer.constant`.
 For example, we can retrieve
 
     >>> snorer.constant.me      # electron mas, MeV
     0.511
     >>> snorer.constant.kpc2cm  # kpc to cm
     3.085e+21
 
@@ -74,90 +83,92 @@
     >>> Tx,mx = 15,0.075
     >>> snorer.get_vx(Tx,mx)
     0.9999876239921284
 
 
 ### SN*ν* BDM Flux 
 
-The BDM flux, or *afterglow* to the ${\rm SN}\nu$, due to SN that is $R_\star$ distant away from us can be evaluated by 
+The BDM flux, or *afterglow* to the ${\rm SN}\nu$, due to SN exploded at $R_\star$ distant away from us can be evaluated by 
 
 $$
 \frac{d\Phi_{\chi}(T_\chi, t^\prime)}{dT_{\chi}dt} =
 \tau\int_0^{2\pi} d\phi\int_{0}^{\pi/2}\sin\theta d\theta~ \mathcal{J} j_{\chi}(r(\phi),D,T_{\chi},\psi)
 $$
 
 where $t$ is the BDM ToF with time-zero at the discovery of SN*ν* on Earth and $t^\prime$ is the total time. We focus on $t$ instead of $t^\prime$.
 Zenith angle $\theta$ and azimuthal angle $\phi$ are relative to the SN-Earth line-of-sight. The default DM-*ν* cross section is $\sigma_{\chi\nu}=10^{-45}$ cm<sup>2</sup>.
 
-The function to evaluate this flux is `snorer.flux()` with $(t,T_\chi,m_\chi,R_\star,\beta)$ are the necessary inputs. 
-Suppose SN's location is at GC, we have $R_\star=8.5$ kpc and $\beta=0$, and examine the flux with turning on DM spike feature
+The function to evaluate this is `snorer.flux()` with $(t,T_\chi,m_\chi,R_\star,\beta)$ are the necessary inputs. 
+Suppose SN's location is at GC, we have $R_\star=8.5$ kpc and $\beta=0$, with default GC-Earth distance $R_e=8.5$ kpc, too.
+With DM spike included, the BDM flux can be calcualted
 
     >>> t,Tx,mx,Rstar,beta = 100,15,1e-2,8.5,0
-    >>> snorer.flux(t,Tx,mx,Rstar,beta,neval=15000)
+    >>> snorer.flux(t,Tx,mx,Rstar,beta,is_spike=True,neval=15000)
     4.572295175982701e-16
 
-Users can turn off the spike feature by inserting `is_spike=False` and will find both numerical results are similar. It implies the contribution to the BDM flux is due to the place outside the spike's influencial region.
+Users can of course turn off the spike feature by setting `is_spike=False` and will find both numerical results are similar.
+It implies the contribution to the BDM flux comes from the place outside the spike's influence.
 
 ### SN*ν* BDM Event
 
 The BDM event number in a detector after exposing to the flux for a period of time, $(t_{\rm min},t_{\rm max})$, can be evaluated by
 
 $$
 N_{\rm BDM} = \int_{t_{\rm min}}^{\rm t_{\rm max}} dt \int_{T_{\chi,{\rm min}}}^{T_{\chi,{\rm max}}}
 \frac{d\Phi_{\chi}(T_\chi, t^\prime)}{dT_{\chi}dt} \times N_e \sigma_{\chi e}
 $$
 
 where $N_e$ is the total electron number in the detector and $\sigma_{\chi e}$ the DM-*e* cross section.
-This can be accomplished by `snorer.event()` with $(m_\chi,R_\star,\beta)$ the necessary inputs.
+This task can be accomplished by `snorer.event()` with $(m_\chi,R_\star,\beta)$ the necessary inputs.
 The default $(t_{\rm min},t_{\rm max})=(10~{\rm s},35~{\rm yrs})$ and $(T_{\chi,{\rm min}},T_{\chi,{\rm max}})=(5,30)$ MeV.
 
 Note that this function is normalized to $N_e=1$ and $\sigma_{\chi e}=1$ cm<sup>2</sup>.
 To have the correct $N_{\rm BDM}$ in a specific detector, users have to mutiply the corresponding $N_e$ and $\sigma_{\chi e}$.
 
 Now let $m_\chi=0.015$ MeV,
 
     >>> mx,Rstar,beta = 0.015,8,0
     >>> N_BDM = snorer.event(mx,Rstar,beta,is_spike=False,neval=50000)
     >>> N_BDM
     1.662174035857532e-06
 
-Suppose it happened in Super-Kamiokande with $N_e\approx 7\times 10^{33}$ and assume $\sigma_{\chi e}=10^{-30}$ cm<sup>2</sup>. The correct $N_{\rm BDM}$ would be
+For Super-Kamiokande, it has $N_e\approx 7\times 10^{33}$ and assume $\sigma_{\chi e}=10^{-35}$ cm<sup>2</sup>. The associated $N_{\rm BDM}$ is
 
     >>> Ne,sigma_xe = 7e33,1e-35
     >>> N_BDM*Ne*sigma_xe
     1.1635218251002724e-07
 
 ### *Experimental* :: Implementation of Particle Physics Model and SN in Arbitrary Distant Galaxy
 
-The aforementioned functions for evaluating BDM signatures are based on model-agnostic picture. It means the cross sections between dark and visble sectors are generally independent of any physical quantities, eg. energy, mass and coupling constants.
+The aforementioned functions for evaluating BDM signatures are based on model-agnostic picture. It means the cross sections between dark and visble sectors are generally independent of physical quantities, eg. energy, mass and coupling constants.
 
-The most important feature of `snorer` is that it offers a general interface for users to implement their favorite particle models.
-Furthermore, SN is not necessary residing in MW or LMC. As long as users can provide these celetial objects' coordinates expressed in *ICRS J2000.0* system, `snorer` can do the calculation.
+The most important feature `snorer` carries is that it offers a general interface for users to implement their favorite particle models.
+Furthermore, SN is not necessary exploding in our MW or LMC. As long as users can provide these celetial objects' coordinates and expressed them in *ICRS J2000.0* metrics, `snorer` can do the calculation.
 `snorer` also allows users to customize the halo shape, by manipulating $\rho_s$, $r_s$ and $n$...etc, and including or excluding spike feature, of such distant galaxy.
 
-This will be done by introducing a *class* `snorer.GeneralInterface`.
-All these user-specified features will compose an instance of `snorer.GeneralInterface`.
+This will be done by the *class* `snorer.GeneralInterface`.
+All these user-specified features will be composed into an instance of `snorer.GeneralInterface`.
 The BDM signatures can be evaluated by calling the associated *methods* within it.
 We have an example in `examples/tutorial.ipynb`, also see the in-class docstring for more information.
 
 
-### Other Useful Functions Classes
+### Other Useful Functions and Classes
 
 We also provide many useful functions and classes at users' disposal. See `examples/tutorial.ipynb` for details.
 
 ## Known Issue
 
 To evaluate BDM event, `snorer` uses `vegas` to handle the multidimensional integration.
-The sampling method of `vegas` cannot manipulate`snorer.event()` as well as the method in the instance of `snorer.GeneralInterface` properly, when SN is exactly at GC with spike feature turning on and no DM self-annihilation.
+The sampling method of `vegas` cannot manipulate event calculation, e.g. `snorer.event()` and the method in the instance of `snorer.GeneralInterface`, properly, when SN is exactly at GC with spike and no DM self-annihilation.
 
 Since the spike is a highly singular behavior, the sampling method may miss the substantial DM contribution from the inner galactic region and causes underestimate of $N_{\rm BDM}$ plus unstable results. 
-To avoid this, users may try to displace the SN from GC when evaluating $N_{\rm BDM}$ whith DM sipke turning on and no DM annihilation.
+To avoid this, users may try to displace the SN from GC a little bit when evaluating $N_{\rm BDM}$ with DM sipke and no DM annihilation.
 For BDM flux evaluation, there is no such issue.
 
 To be fair, the probability of a very cuspy DM spike surving the gravitational disturbance without annihilating away and SN happening exactly at the GC might be very rare.
 
-This issue is scheduled to fix in the next version of `snorer`.
+This issue is scheduled to fix in the next major update of `snorer`.
 
 ## Bugs and troubleshooting
 
 Please report to the author, Yen-Hsun Lin, via [yenhsun@phys.ncku.edu.tw](mailto:yenhsun@phys.ncku.edu.tw).
```

### Comparing `snorer-1.0.0/pyproject.toml` & `snorer-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "snorer"
-version = "1.0.0"
+version = "1.0.1"
 description = "This package evaluates the time-of-flight signatures of boosted dark matter due to supernova neutrinos from our Milky Way"
 readme = "README.md"
 authors = [{ name = "Yen-Hsun Lin", email = "yenhsun@phys.ncku.edu.tw" }]
 license = { file = "LICENSE" }
 dependencies = [
     "numpy >= 1.20.0",
     "scipy >= 1.10.0",
@@ -16,15 +16,15 @@
     "astropy >= 6.0.0",]
 requires-python = ">=3.8"
 
 [project.urls]
 Homepage = "https://github.com/yenhsunlin/snorer"
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `snorer-1.0.0/src/snorer/__init__.py` & `snorer-1.0.1/src/snorer/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 """
 This is the proxy script
 """
 
 
 __name__         = 'snorer'
-__version__      = '1.0.0'
+__version__      = '1.0.1'
 __description__  = 'This package evaluates the time-of-flight signatures of boosted dark matter due to supernova neutrinos from our Milky Way, SN1987a in LMC or from SN in arbitrary distant galaxy'
 __author__       = 'Yen-Hsun Lin'
 __email__        = 'yenhsun@phys.ncku.edu.tw'
 __url__          = 'https://github.com/yenhsunlin/snorer'
 __license__      = 'GNU GPL-3.0'
 __all__          = ['snNuSpectrum','dsigma_xv','emissivity','diff_flux','flux','event',
                     'HaloSpike','rhox','M_sigma','radiusInfluence','radiusSchwarzschild','dmNumberDensity',
```

### Comparing `snorer-1.0.0/src/snorer/constants.py` & `snorer-1.0.1/src/snorer/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     
     @property
     def LMC_coord(self):       # LMC's RA, DEC and distance
         return ['05h23m34.5264s', '-69d45m22.053s',49.97]
     
     @property
     def SN1987a_coord(self):   # SN1987a's RA, DEC and distance
-        return ['05h35m27.8733s', '-69d16m10.478s',51.7]
+        return ['05h35m27.8733s', '-69d16m10.478s',51.4]
 
     @property
     def MW_profile(self):      # Profile parameters for MW
         return {'rhos':184,'rs':24.42,'n':2,'mBH':self.M_SgrA,'rh':2e-3}
     
     @property
     def LMC_profile(self):      # Profile parameters for LMC
```

### Comparing `snorer-1.0.0/src/snorer/geometry.py` & `snorer-1.0.1/src/snorer/geometry.py`

 * *Files identical despite different names*

### Comparing `snorer-1.0.0/src/snorer/halo.py` & `snorer-1.0.1/src/snorer/halo.py`

 * *Files identical despite different names*

### Comparing `snorer-1.0.0/src/snorer/kinematics.py` & `snorer-1.0.1/src/snorer/kinematics.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,49 +135,62 @@
     def __init__(self,m1,m2,T2,psi):
         self.m1 = m1
         self.m2 = m2
         self.T2 = T2
         self.psi = psi
 
     @property
-    def _x(self):
+    def x(self):
         return cos(self.psi)
     
     def get_sanity(self) -> bool:
-        return self.get_T1() >= 0 
+        T2,m2,x = self.T2,self.m2,self.x
+        return T2 < sqrt(T2*(T2+2*m2))*x
+        #return self.get_T1() >= 0 
     
     def get_T1(self) -> float:
-        T2,m1,m2,x = self.T2,self.m1,self.m2,self._x
+        T2,m1,m2,x = self.T2,self.m1,self.m2,self.x
+        # Mathematica generated expression
         p2sq = T2*(T2+2*m2)
         # Mathematica generated expression
         numerator = sqrt(m1**2*p2sq**2*x**4 + p2sq*T2**2*x**2*(m2**2-m1**2)) + m2*T2**2
         denominator = p2sq*x**2 - T2**2
         return numerator/denominator - m1
+        
+        # following expressions may yield invalid value in sqrt
+        # numerator = (2*m1*T2+2*m2*T2-4*m1*m2*x**2-2*m1*T2*x**2+sqrt(-4*(-m1**2*T2-2*m1*m2*T2  \
+        #              -m2**2*T2)*(-T2+2*m2*x**2+T2*x**2)+(-2*m1*T2-2*m2*T2+4*m1*m2*x**2        \
+        #              +2*m1*T2*x**2)**2))
+        # denominator = (2*(-T2+2*m2*x**2+T2*x**2))
+        # return numerator/denominator
 
     def get_dT1(self) -> float:
-        T2,m1,m2,x = self.T2,self.m1,self.m2,self._x
+        T2,m1,m2,x = self.T2,self.m1,self.m2,self.x
         # Mathematica generated expression
-        numerator = (m2*x**2*(m1**2*T2*(-T2+(2*m2+T2)*x**2)+m2*(m2*T2*(T2+(2*m2+T2)*x**2)+2*sqrt(T2**2*(2*m2+T2)*x**2*(m2**2*T2+m1**2*(-T2+(2*m2+T2)*x**2))))))
-        denominator = ((T2-(2*m2+T2)*x**2)**2*sqrt(T2**2*(2*m2+T2)*x**2*(m2**2*T2+m1**2*(-T2+(2*m2+T2)*x**2))))
+        numerator = (m2*x**2*(m1**2*T2*(-T2+(2*m2+T2)*x**2)+m2*(m2*T2*(T2+(2*m2+T2)*x**2)+    \
+                     2*sqrt(T2**2*(2*m2+T2)*x**2*(m2**2*T2+m1**2*(-T2+(2*m2+T2)*x**2)))))) 
+        denominator = ((T2-(2*m2+T2)*x**2)**2*sqrt(T2**2*(2*m2+T2)*x**2*(m2**2*T2+m1**2       \
+                      *(-T2+(2*m2+T2)*x**2))))
         return numerator/denominator
 
     def get_dLips(self) -> float:
         T1,m1,m2 = self.get_T1(),self.m1,self.m2
         s = m1**2 + m2**2 + 2*m2*(T1 + m1)
         psq = (s - (m1+m2)**2)*(s-(m1-m2)**2)/4/s
         return abs(self._du_dx()/64/pi/s/psq/2/pi)
 
     def _du_dx(self) -> float:
-        T2,m1,m2,x = self.T2,self.m1,self.m2,self._x
+        T2,m1,m2,x = self.T2,self.m1,self.m2,self.x
         E1 = self.get_T1() + m1
         E2 = T2 + m2
         p2sq = T2*(T2+2*m2)
         p2 = sqrt(p2sq)
         # Mathematica generated expression
-        num = (p2sq*T2**2*x*((m1-m2)*(m1+m2)*T2**2-(m1**2+m2**2)*p2sq*x**2-2*m2*sqrt((-m1**2+m2**2)*p2sq*T2**2*x**2+m1**2*p2sq**2*x**4)))
+        num = (p2sq*T2**2*x*((m1-m2)*(m1+m2)*T2**2-(m1**2+m2**2)*p2sq*x**2-2*m2*sqrt((-m1**2  \
+               +m2**2)*p2sq*T2**2*x**2+m1**2*p2sq**2*x**4)))
         den = ((T2-p2*x)**2*(T2+p2*x)**2*sqrt((-m1**2+m2**2)*p2sq*T2**2*x**2+m1**2*p2sq**2*x**4))
         return -2*(num/den)*(E2 - p2*x) + 2*E1*p2
 
 
 class Mandelstam(Kinematics):
     """
     Superclass: Kinematics
```

### Comparing `snorer-1.0.0/src/snorer/snorerMain.py` & `snorer-1.0.1/src/snorer/snorerMain.py`

 * *Files identical despite different names*

### Comparing `snorer-1.0.0/src/snorer/sysmsg.py` & `snorer-1.0.1/src/snorer/sysmsg.py`

 * *Files identical despite different names*

### Comparing `snorer-1.0.0/src/snorer/utils.py` & `snorer-1.0.1/src/snorer/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,23 +388,23 @@
         Output
         ------
         scalar: The diff. BDM flux at Earth, # per MeV per cm^2 per second
     
         See Eq. (6) in Phys. Rev. D 108, 083013 (2023) 
         """
         Rstar = self.Rstar
-        _,t_van = get_tof(Tx,mx,Rstar)                           # get the vanishing time t_van 
-        if t <= t_van:
-            theta_min,theta_max = get_thetaRange(t,Tx,mx,Rstar)  # get the zenith angle range that contains non-zero BDM flux
-            integ = vegas.Integrator([[theta_min,theta_max],[0,2*pi]])  # (theta,phi)
-            flux = integ(lambda x: self._diff_flux(t=t,Tx=Tx,mx=mx,theta=x[0],phi=x[1],tau=tau),
-                         nitn=nitn,neval=neval).mean
-            return flux
-        else:                                                    # t > t_van will yield zero BDM
-            return 0
+        # _,t_van = get_tof(Tx,mx,Rstar)                           # get the vanishing time t_van 
+        # if t <= t_van:
+        theta_min,theta_max = get_thetaRange(t,Tx,mx,Rstar)  # get the zenith angle range that contains non-zero BDM flux
+        integ = vegas.Integrator([[theta_min,theta_max],[0,2*pi]])  # (theta,phi)
+        flux = integ(lambda x: self._diff_flux(t=t,Tx=Tx,mx=mx,theta=x[0],phi=x[1],tau=tau),
+                        nitn=nitn,neval=neval).mean
+        return flux
+        # else:                                                    # t > t_van will yield zero BDM
+        #     return 0
     
     def event(self,mx,TxRange=[5,30],tRange=[10,35*constant.year2Seconds],tau=10,
               nitn=10,neval=30000) -> float:
         """
         The SNv BDM evnet at Earth after integrated over exposure time t, BDM
         kinetic energy Tx, zenith angle theta and azimuthal angle phi
```

### Comparing `snorer-1.0.0/src/snorer.egg-info/PKG-INFO` & `snorer-1.0.1/src/snorer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snorer
-Version: 1.0.0
+Version: 1.0.1
 Summary: This package evaluates the time-of-flight signatures of boosted dark matter due to supernova neutrinos from our Milky Way
 Author-email: Yen-Hsun Lin <yenhsun@phys.ncku.edu.tw>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -691,31 +691,40 @@
 <a href = "https://choosealicense.com/licenses/gpl-3.0/"  target = "_blank">![License](https://img.shields.io/badge/License-GPL_3.0-blue.svg)</a>
 <a href = "https://arxiv.org/abs/2206.06864"  target = "_blank">![ArXiv](https://img.shields.io/badge/arXiv-2206.06864-yellowgreen.svg)</a>
 <a href = "https://arxiv.org/abs/2307.03522"  target = "_blank">![ArXiv](https://img.shields.io/badge/arXiv-2307.03522-yellowgreen.svg)</a>
 
 # snorer: *S*upernova-*N*eutrino-b*O*osted da*R*k matt*ER*
 
 
-`snorer` is a package for evaluating time-of-flight signatures of supernova-neutrino-boosted dark matter (SN*ν* BDM) from our Milky Way (MW) and SN1987a in Large Magellanic Cloud (LMC) based on
+`snorer` is a package for evaluating time-of-flight signatures of supernova-neutrino-boosted dark matter (SN*ν* BDM) from our Milky Way (MW), SN1987a in Large Magellanic Cloud (LMC) and SN in arbitrary distant galaxy based on
 <a href = "https://doi.org/10.1103/PhysRevLett.130.111002" target = "_blank">*Phys. Rev. Lett.* **130**, 111002 (2023)</a> [<a href = "https://arxiv.org/abs/2206.06864" target = "_blank">arXiv:2206.06864</a>]
 and
 <a href = "https://doi.org/10.1103/PhysRevD.108.083013" target = "_blank">*Phys. Rev. D* **108**, 083013 (2023)</a>
 [<a href = "https://arxiv.org/abs/2307.03522" target = "_blank">arXiv:2307.03522</a>].
 
+### Citation
+
+If you use this package or part of the code in your research, please cite the followings:
+
+1. Y.-H. Lin *et al.*, *Phys. Rev. Lett.* **130**, 111002 (2023), arXiv:2206.06864
+2. Y.-H. Lin *et al.*, *Phys. Rev. D* **108**, 083013 (2023), arXiv:2307.03522
+3. `snorer`: https://github.com/yenhsunlin/snorer
+
+
 ## Installation
 
 To install, excute the following command on the prompt
 
     $ pip install snorer
 
 and everything should be processed on-the-fly.
 
 ### Dependency
 
-`snorer` requires python >= 3.8 and the following packages these external packages
+`snorer` requires python >= 3.8 and the following external packages
 
 - `numpy` >= 1.20.0
 - `scipy` >= 1.10.0
 - `vegas` >= 6.0.1
 - `astropy` >= 6.0.0
 
 where `vegas` is a the backend engine for evaluating multidimensional integrals based on adaptive Monte Carlo vegas algorithm, see its homepage: <a heref = "https://pypi.org/project/vegas/" target = "_blank">https://pypi.org/project/vegas/</a>.
@@ -728,22 +737,22 @@
 We briefly summarize the usage in this section and a comprehensive tutorial can be found in the jupyter notebook in `examples/tutorial.ipynb`.
 
 To import, do
 
     >>> import snorer
 
 in python terminal and is similar in the jupyter notebook.
-All functions and classes can be accessed by typing `snorer.foo()` where `foo` is the name.
+All functions and classes can be accessed by typing `snorer.foo()` where `foo` is the function/class/module name.
 
 
 
 
 ### Useful Constants
 
-We document various useful physical constants and conversion factors...etc as the *attributes* of an instance `snorer.constant`.
+We document various useful physical constants and conversion factors...etc as the *attributes* of the instance `snorer.constant`.
 For example, we can retrieve
 
     >>> snorer.constant.me      # electron mas, MeV
     0.511
     >>> snorer.constant.kpc2cm  # kpc to cm
     3.085e+21
 
@@ -763,90 +772,92 @@
     >>> Tx,mx = 15,0.075
     >>> snorer.get_vx(Tx,mx)
     0.9999876239921284
 
 
 ### SN*ν* BDM Flux 
 
-The BDM flux, or *afterglow* to the ${\rm SN}\nu$, due to SN that is $R_\star$ distant away from us can be evaluated by 
+The BDM flux, or *afterglow* to the ${\rm SN}\nu$, due to SN exploded at $R_\star$ distant away from us can be evaluated by 
 
 $$
 \frac{d\Phi_{\chi}(T_\chi, t^\prime)}{dT_{\chi}dt} =
 \tau\int_0^{2\pi} d\phi\int_{0}^{\pi/2}\sin\theta d\theta~ \mathcal{J} j_{\chi}(r(\phi),D,T_{\chi},\psi)
 $$
 
 where $t$ is the BDM ToF with time-zero at the discovery of SN*ν* on Earth and $t^\prime$ is the total time. We focus on $t$ instead of $t^\prime$.
 Zenith angle $\theta$ and azimuthal angle $\phi$ are relative to the SN-Earth line-of-sight. The default DM-*ν* cross section is $\sigma_{\chi\nu}=10^{-45}$ cm<sup>2</sup>.
 
-The function to evaluate this flux is `snorer.flux()` with $(t,T_\chi,m_\chi,R_\star,\beta)$ are the necessary inputs. 
-Suppose SN's location is at GC, we have $R_\star=8.5$ kpc and $\beta=0$, and examine the flux with turning on DM spike feature
+The function to evaluate this is `snorer.flux()` with $(t,T_\chi,m_\chi,R_\star,\beta)$ are the necessary inputs. 
+Suppose SN's location is at GC, we have $R_\star=8.5$ kpc and $\beta=0$, with default GC-Earth distance $R_e=8.5$ kpc, too.
+With DM spike included, the BDM flux can be calcualted
 
     >>> t,Tx,mx,Rstar,beta = 100,15,1e-2,8.5,0
-    >>> snorer.flux(t,Tx,mx,Rstar,beta,neval=15000)
+    >>> snorer.flux(t,Tx,mx,Rstar,beta,is_spike=True,neval=15000)
     4.572295175982701e-16
 
-Users can turn off the spike feature by inserting `is_spike=False` and will find both numerical results are similar. It implies the contribution to the BDM flux is due to the place outside the spike's influencial region.
+Users can of course turn off the spike feature by setting `is_spike=False` and will find both numerical results are similar.
+It implies the contribution to the BDM flux comes from the place outside the spike's influence.
 
 ### SN*ν* BDM Event
 
 The BDM event number in a detector after exposing to the flux for a period of time, $(t_{\rm min},t_{\rm max})$, can be evaluated by
 
 $$
 N_{\rm BDM} = \int_{t_{\rm min}}^{\rm t_{\rm max}} dt \int_{T_{\chi,{\rm min}}}^{T_{\chi,{\rm max}}}
 \frac{d\Phi_{\chi}(T_\chi, t^\prime)}{dT_{\chi}dt} \times N_e \sigma_{\chi e}
 $$
 
 where $N_e$ is the total electron number in the detector and $\sigma_{\chi e}$ the DM-*e* cross section.
-This can be accomplished by `snorer.event()` with $(m_\chi,R_\star,\beta)$ the necessary inputs.
+This task can be accomplished by `snorer.event()` with $(m_\chi,R_\star,\beta)$ the necessary inputs.
 The default $(t_{\rm min},t_{\rm max})=(10~{\rm s},35~{\rm yrs})$ and $(T_{\chi,{\rm min}},T_{\chi,{\rm max}})=(5,30)$ MeV.
 
 Note that this function is normalized to $N_e=1$ and $\sigma_{\chi e}=1$ cm<sup>2</sup>.
 To have the correct $N_{\rm BDM}$ in a specific detector, users have to mutiply the corresponding $N_e$ and $\sigma_{\chi e}$.
 
 Now let $m_\chi=0.015$ MeV,
 
     >>> mx,Rstar,beta = 0.015,8,0
     >>> N_BDM = snorer.event(mx,Rstar,beta,is_spike=False,neval=50000)
     >>> N_BDM
     1.662174035857532e-06
 
-Suppose it happened in Super-Kamiokande with $N_e\approx 7\times 10^{33}$ and assume $\sigma_{\chi e}=10^{-30}$ cm<sup>2</sup>. The correct $N_{\rm BDM}$ would be
+For Super-Kamiokande, it has $N_e\approx 7\times 10^{33}$ and assume $\sigma_{\chi e}=10^{-35}$ cm<sup>2</sup>. The associated $N_{\rm BDM}$ is
 
     >>> Ne,sigma_xe = 7e33,1e-35
     >>> N_BDM*Ne*sigma_xe
     1.1635218251002724e-07
 
 ### *Experimental* :: Implementation of Particle Physics Model and SN in Arbitrary Distant Galaxy
 
-The aforementioned functions for evaluating BDM signatures are based on model-agnostic picture. It means the cross sections between dark and visble sectors are generally independent of any physical quantities, eg. energy, mass and coupling constants.
+The aforementioned functions for evaluating BDM signatures are based on model-agnostic picture. It means the cross sections between dark and visble sectors are generally independent of physical quantities, eg. energy, mass and coupling constants.
 
-The most important feature of `snorer` is that it offers a general interface for users to implement their favorite particle models.
-Furthermore, SN is not necessary residing in MW or LMC. As long as users can provide these celetial objects' coordinates expressed in *ICRS J2000.0* system, `snorer` can do the calculation.
+The most important feature `snorer` carries is that it offers a general interface for users to implement their favorite particle models.
+Furthermore, SN is not necessary exploding in our MW or LMC. As long as users can provide these celetial objects' coordinates and expressed them in *ICRS J2000.0* metrics, `snorer` can do the calculation.
 `snorer` also allows users to customize the halo shape, by manipulating $\rho_s$, $r_s$ and $n$...etc, and including or excluding spike feature, of such distant galaxy.
 
-This will be done by introducing a *class* `snorer.GeneralInterface`.
-All these user-specified features will compose an instance of `snorer.GeneralInterface`.
+This will be done by the *class* `snorer.GeneralInterface`.
+All these user-specified features will be composed into an instance of `snorer.GeneralInterface`.
 The BDM signatures can be evaluated by calling the associated *methods* within it.
 We have an example in `examples/tutorial.ipynb`, also see the in-class docstring for more information.
 
 
-### Other Useful Functions Classes
+### Other Useful Functions and Classes
 
 We also provide many useful functions and classes at users' disposal. See `examples/tutorial.ipynb` for details.
 
 ## Known Issue
 
 To evaluate BDM event, `snorer` uses `vegas` to handle the multidimensional integration.
-The sampling method of `vegas` cannot manipulate`snorer.event()` as well as the method in the instance of `snorer.GeneralInterface` properly, when SN is exactly at GC with spike feature turning on and no DM self-annihilation.
+The sampling method of `vegas` cannot manipulate event calculation, e.g. `snorer.event()` and the method in the instance of `snorer.GeneralInterface`, properly, when SN is exactly at GC with spike and no DM self-annihilation.
 
 Since the spike is a highly singular behavior, the sampling method may miss the substantial DM contribution from the inner galactic region and causes underestimate of $N_{\rm BDM}$ plus unstable results. 
-To avoid this, users may try to displace the SN from GC when evaluating $N_{\rm BDM}$ whith DM sipke turning on and no DM annihilation.
+To avoid this, users may try to displace the SN from GC a little bit when evaluating $N_{\rm BDM}$ with DM sipke and no DM annihilation.
 For BDM flux evaluation, there is no such issue.
 
 To be fair, the probability of a very cuspy DM spike surving the gravitational disturbance without annihilating away and SN happening exactly at the GC might be very rare.
 
-This issue is scheduled to fix in the next version of `snorer`.
+This issue is scheduled to fix in the next major update of `snorer`.
 
 ## Bugs and troubleshooting
 
 Please report to the author, Yen-Hsun Lin, via [yenhsun@phys.ncku.edu.tw](mailto:yenhsun@phys.ncku.edu.tw).
```

