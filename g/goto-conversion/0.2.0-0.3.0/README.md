# Comparing `tmp/goto_conversion-0.2.0.tar.gz` & `tmp/goto_conversion-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goto_conversion-0.2.0.tar", last modified: Fri Apr 12 05:59:49 2024, max compression
+gzip compressed data, was "goto_conversion-0.3.0.tar", last modified: Thu May  2 09:49:03 2024, max compression
```

## Comparing `goto_conversion-0.2.0.tar` & `goto_conversion-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-04-12 05:59:49.729019 goto_conversion-0.2.0/
--rw-rw-r--   0 gotoukaijin   (501) staff       (20)     1073 2024-04-12 05:54:23.000000 goto_conversion-0.2.0/LICENSE.txt
--rw-r--r--   0 gotoukaijin   (501) staff       (20)     5561 2024-04-12 05:59:49.728235 goto_conversion-0.2.0/PKG-INFO
--rw-rw-r--   0 gotoukaijin   (501) staff       (20)     5032 2024-04-12 05:54:23.000000 goto_conversion-0.2.0/README.md
--rw-rw-r--   0 gotoukaijin   (501) staff       (20)      596 2024-04-12 05:54:23.000000 goto_conversion-0.2.0/pyproject.toml
--rw-r--r--   0 gotoukaijin   (501) staff       (20)       38 2024-04-12 05:59:49.729164 goto_conversion-0.2.0/setup.cfg
-drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-04-12 05:59:49.722608 goto_conversion-0.2.0/src/
-drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-04-12 05:59:49.727434 goto_conversion-0.2.0/src/goto_conversion.egg-info/
--rw-r--r--   0 gotoukaijin   (501) staff       (20)     5561 2024-04-12 05:59:49.000000 goto_conversion-0.2.0/src/goto_conversion.egg-info/PKG-INFO
--rw-r--r--   0 gotoukaijin   (501) staff       (20)      208 2024-04-12 05:59:49.000000 goto_conversion-0.2.0/src/goto_conversion.egg-info/SOURCES.txt
--rw-r--r--   0 gotoukaijin   (501) staff       (20)        1 2024-04-12 05:59:49.000000 goto_conversion-0.2.0/src/goto_conversion.egg-info/dependency_links.txt
--rw-r--r--   0 gotoukaijin   (501) staff       (20)        1 2024-04-12 05:59:49.000000 goto_conversion-0.2.0/src/goto_conversion.egg-info/top_level.txt
+drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-05-02 09:49:03.291061 goto_conversion-0.3.0/
+-rw-rw-r--   0 gotoukaijin   (501) staff       (20)     1073 2024-05-02 09:39:25.000000 goto_conversion-0.3.0/LICENSE.txt
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)     6895 2024-05-02 09:49:03.290870 goto_conversion-0.3.0/PKG-INFO
+-rw-rw-r--   0 gotoukaijin   (501) staff       (20)     6348 2024-05-02 09:39:25.000000 goto_conversion-0.3.0/README.md
+-rw-rw-r--   0 gotoukaijin   (501) staff       (20)      614 2024-05-02 09:39:25.000000 goto_conversion-0.3.0/pyproject.toml
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)       38 2024-05-02 09:49:03.291103 goto_conversion-0.3.0/setup.cfg
+drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-05-02 09:49:03.289043 goto_conversion-0.3.0/src/
+drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-05-02 09:49:03.289740 goto_conversion-0.3.0/src/goto_conversion/
+-rw-rw-r--   0 gotoukaijin   (501) staff       (20)     1639 2024-05-02 09:39:25.000000 goto_conversion-0.3.0/src/goto_conversion/__init__.py
+drwxr-xr-x   0 gotoukaijin   (501) staff       (20)        0 2024-05-02 09:49:03.290626 goto_conversion-0.3.0/src/goto_conversion.egg-info/
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)     6895 2024-05-02 09:49:03.000000 goto_conversion-0.3.0/src/goto_conversion.egg-info/PKG-INFO
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)      240 2024-05-02 09:49:03.000000 goto_conversion-0.3.0/src/goto_conversion.egg-info/SOURCES.txt
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)        1 2024-05-02 09:49:03.000000 goto_conversion-0.3.0/src/goto_conversion.egg-info/dependency_links.txt
+-rw-r--r--   0 gotoukaijin   (501) staff       (20)       16 2024-05-02 09:49:03.000000 goto_conversion-0.3.0/src/goto_conversion.egg-info/top_level.txt
```

### Comparing `goto_conversion-0.2.0/LICENSE.txt` & `goto_conversion-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `goto_conversion-0.2.0/PKG-INFO` & `goto_conversion-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 Metadata-Version: 2.1
 Name: goto_conversion
-Version: 0.2.0
-Summary: Novel Conversion of Betting Odds to Probabilities
+Version: 0.3.0
+Summary: Gambling Odds To Outcome probabilities Conversion (goto_conversion)
 Author: Kaito Goto
 Project-URL: Homepage, https://github.com/gotoConversion/goto_conversion
 Project-URL: Bug Tracker, https://github.com/gotoConversion/goto_conversion/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# goto_conversion: Novel Conversion of Betting Odds to Probabilities
+# Gambling Odds To Outcome probabilities Conversion (goto_conversion)
 
 The most common method used to convert betting odds to probabilities is to normalise the inverse odds (Multiplicative conversion). However, this method does not consider the favourite-longshot bias. 
 
 To the best of our knowledge, there are two existing methods that attempt to consider the favourite-longshot bias. (i) Shin conversion [[1](#1),[2](#2),[3](#3)] maximises the expected profit for the bookmakers assuming a small proportion of bettors have inside information. (ii) Power conversion [[4](#4)] raises all inverse odds to the same constant power. However, both of these methods require iterative computation to convert betting odds to probabilities.
 
-Our proposed method (`goto_conversion`) is significantly more efficient than Shin and Power conversion because it converts betting odds to probabilities directly without iterative computation.
+Our proposed method, **G**ambling **O**dds **T**o **O**utcome probabilities **Conversion** (`goto_conversion`) is significantly more efficient than Shin and Power conversion because it converts betting odds to probabilities directly without iterative computation.
 
 The `goto_conversion` reduces all inverse odds by the same units of standard error. This attempts to consider the favourite-longshot bias by utilising the proportionately wider standard errors implied for inverses of longshot odds and vice-versa.
 
 Furthermore, our tables of experiment results show that the `goto_conversion` converts betting odds to probabilities more accurately than all three of these existing methods.
 
 The favourite-longshot bias is not limited to gambling markets, it exists in stock markets too. Thus, we applied the original `goto_conversion` to stock markets by defining the `zero_sum` variant. Under the same philosophy as the original `goto_conversion`, `zero_sum` adjusts all predicted stock prices (e.g. weighted average price) by the same units of standard error to ensure all predicted stock prices relative to the index price (e.g. weighted average nasdaq price) sum to zero. This attempts to consider the favourite-longshot bias by utilising the wider standard errors implied for predicted stock prices with low trade volume and vice-versa.
 
 # Citations (not limited to, unofficial)
 
-[Most Voted Public Solution from 2024 Optiver Kaggle Competition](https://www.kaggle.com/code/ravi20076/optiver-baseline-models?scriptVersionId=152991375)
+[Most Voted Solution from 2023 Optiver Kaggle Competition](https://www.kaggle.com/code/ravi20076/optiver-baseline-models?scriptVersionId=152991375)
 
-[1xGold and 2xSilver Medal Winning Public Solution from 2019 to 2022 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/1xgold-2xsilvers-key-ingredient)
+[Gold Medal Winning (14th out of 3225) Solution from 2023 Optiver Kaggle Competition (the `zero_sum` variant)](https://www.kaggle.com/competitions/optiver-trading-at-the-close/discussion/462653)
 
-[Bronze Medal Winning Public Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/updated-1xgold-2xsilvers-key-ingredient)
+[Gold Medal Winning (3rd out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/495101)
+
+[Gold Medal Winning (4th out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/494407)
+
+[1xGold and 2xSilver Medal Winning Solution from 2019 to 2022 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/1xgold-2xsilvers-key-ingredient)
+
+[15xBronze Medal Winning (86th to 100th place out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/updated-1xgold-2xsilvers-key-ingredient)
 
 # Installation
 
 Requires Python 3.7 or above.
 
 ```
 pip install goto-conversion
@@ -68,26 +74,24 @@
 
 # Pseudo Code
 
 ![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/PseudoCode.png?raw=true)
 
 # Experiment Results
 
-The experiment results table directly below is based on the same 6,000 football matches' betting odds (home win, draw or away win) across four different bookmakers.
+Brier Score was mainly used to evaluate the accuracy of the probabilities implied by each conversion method. The Brier Score is essentially the mean squared error of the probabilities relative to the ground truth. Ranked Probability Score (RPS) was additionally used to evaluate the probabilities for football betting odds because the outcome is ordinal (home win, draw and away win). RPS is essentially the Brier Score on the cumulative probabilities.
 
-![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/FballExperiment.png?raw=true)
+The experiment results table directly below is based on the same 6,000 football matches' betting odds (home win, draw or away win) across four different bookmakers. `goto_conversion` outperforms all other conversion methods for all four bookmakers. Kaggle notebook to reproduce the table directly below can be found [here](https://www.kaggle.com/code/kaito510/novel-conversion-of-football-betting-odds).
 
-Kaggle notebook to reproduce the table directly above: https://www.kaggle.com/code/kaito510/novel-conversion-of-football-betting-odds
+![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/FballExperiment.png?raw=true)
 
-The experiment results table directly below is based on 6,348 horse races' betting odds for the win and place markets.
+The experiment results table directly below is based on 6,348 horse races' betting odds for the win and place markets. `goto_conversion` outperforms all other conversion methods for both win and place betting markets. Kaggle notebook to reproduce the table directly below can be found [here](https://www.kaggle.com/code/kaito510/novel-conversion-of-horse-racing-odds).
 
 ![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/RacingExperiment.png?raw=true)
 
-Kaggle notebook to reproduce the table directly above: https://www.kaggle.com/code/kaito510/novel-conversion-of-horse-racing-odds
-
 # References
 
 <a id="1">[1]</a> 
 [H. S. Shin, “Prices of State Contingent Claims with Insider
 traders, and the Favorite-Longshot Bias”. The Economic
 Journal, 1992, 102, pp. 426-435.](https://doi.org/10.2307/2234526)
```

### Comparing `goto_conversion-0.2.0/README.md` & `goto_conversion-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,34 @@
-# goto_conversion: Novel Conversion of Betting Odds to Probabilities
+# Gambling Odds To Outcome probabilities Conversion (goto_conversion)
 
 The most common method used to convert betting odds to probabilities is to normalise the inverse odds (Multiplicative conversion). However, this method does not consider the favourite-longshot bias. 
 
 To the best of our knowledge, there are two existing methods that attempt to consider the favourite-longshot bias. (i) Shin conversion [[1](#1),[2](#2),[3](#3)] maximises the expected profit for the bookmakers assuming a small proportion of bettors have inside information. (ii) Power conversion [[4](#4)] raises all inverse odds to the same constant power. However, both of these methods require iterative computation to convert betting odds to probabilities.
 
-Our proposed method (`goto_conversion`) is significantly more efficient than Shin and Power conversion because it converts betting odds to probabilities directly without iterative computation.
+Our proposed method, **G**ambling **O**dds **T**o **O**utcome probabilities **Conversion** (`goto_conversion`) is significantly more efficient than Shin and Power conversion because it converts betting odds to probabilities directly without iterative computation.
 
 The `goto_conversion` reduces all inverse odds by the same units of standard error. This attempts to consider the favourite-longshot bias by utilising the proportionately wider standard errors implied for inverses of longshot odds and vice-versa.
 
 Furthermore, our tables of experiment results show that the `goto_conversion` converts betting odds to probabilities more accurately than all three of these existing methods.
 
 The favourite-longshot bias is not limited to gambling markets, it exists in stock markets too. Thus, we applied the original `goto_conversion` to stock markets by defining the `zero_sum` variant. Under the same philosophy as the original `goto_conversion`, `zero_sum` adjusts all predicted stock prices (e.g. weighted average price) by the same units of standard error to ensure all predicted stock prices relative to the index price (e.g. weighted average nasdaq price) sum to zero. This attempts to consider the favourite-longshot bias by utilising the wider standard errors implied for predicted stock prices with low trade volume and vice-versa.
 
 # Citations (not limited to, unofficial)
 
-[Most Voted Public Solution from 2024 Optiver Kaggle Competition](https://www.kaggle.com/code/ravi20076/optiver-baseline-models?scriptVersionId=152991375)
+[Most Voted Solution from 2023 Optiver Kaggle Competition](https://www.kaggle.com/code/ravi20076/optiver-baseline-models?scriptVersionId=152991375)
 
-[1xGold and 2xSilver Medal Winning Public Solution from 2019 to 2022 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/1xgold-2xsilvers-key-ingredient)
+[Gold Medal Winning (14th out of 3225) Solution from 2023 Optiver Kaggle Competition (the `zero_sum` variant)](https://www.kaggle.com/competitions/optiver-trading-at-the-close/discussion/462653)
 
-[Bronze Medal Winning Public Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/updated-1xgold-2xsilvers-key-ingredient)
+[Gold Medal Winning (3rd out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/495101)
+
+[Gold Medal Winning (4th out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/494407)
+
+[1xGold and 2xSilver Medal Winning Solution from 2019 to 2022 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/1xgold-2xsilvers-key-ingredient)
+
+[15xBronze Medal Winning (86th to 100th place out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/updated-1xgold-2xsilvers-key-ingredient)
 
 # Installation
 
 Requires Python 3.7 or above.
 
 ```
 pip install goto-conversion
@@ -54,26 +60,24 @@
 
 # Pseudo Code
 
 ![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/PseudoCode.png?raw=true)
 
 # Experiment Results
 
-The experiment results table directly below is based on the same 6,000 football matches' betting odds (home win, draw or away win) across four different bookmakers.
+Brier Score was mainly used to evaluate the accuracy of the probabilities implied by each conversion method. The Brier Score is essentially the mean squared error of the probabilities relative to the ground truth. Ranked Probability Score (RPS) was additionally used to evaluate the probabilities for football betting odds because the outcome is ordinal (home win, draw and away win). RPS is essentially the Brier Score on the cumulative probabilities.
 
-![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/FballExperiment.png?raw=true)
+The experiment results table directly below is based on the same 6,000 football matches' betting odds (home win, draw or away win) across four different bookmakers. `goto_conversion` outperforms all other conversion methods for all four bookmakers. Kaggle notebook to reproduce the table directly below can be found [here](https://www.kaggle.com/code/kaito510/novel-conversion-of-football-betting-odds).
 
-Kaggle notebook to reproduce the table directly above: https://www.kaggle.com/code/kaito510/novel-conversion-of-football-betting-odds
+![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/FballExperiment.png?raw=true)
 
-The experiment results table directly below is based on 6,348 horse races' betting odds for the win and place markets.
+The experiment results table directly below is based on 6,348 horse races' betting odds for the win and place markets. `goto_conversion` outperforms all other conversion methods for both win and place betting markets. Kaggle notebook to reproduce the table directly below can be found [here](https://www.kaggle.com/code/kaito510/novel-conversion-of-horse-racing-odds).
 
 ![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/RacingExperiment.png?raw=true)
 
-Kaggle notebook to reproduce the table directly above: https://www.kaggle.com/code/kaito510/novel-conversion-of-horse-racing-odds
-
 # References
 
 <a id="1">[1]</a> 
 [H. S. Shin, “Prices of State Contingent Claims with Insider
 traders, and the Favorite-Longshot Bias”. The Economic
 Journal, 1992, 102, pp. 426-435.](https://doi.org/10.2307/2234526)
```

### Comparing `goto_conversion-0.2.0/pyproject.toml` & `goto_conversion-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "goto_conversion"
-version = "0.2.0"
+version = "0.3.0"
 authors = [{ name = 'Kaito Goto' },]
-description = "Novel Conversion of Betting Odds to Probabilities"
+description = "Gambling Odds To Outcome probabilities Conversion (goto_conversion)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `goto_conversion-0.2.0/src/goto_conversion.egg-info/PKG-INFO` & `goto_conversion-0.3.0/src/goto_conversion.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 Metadata-Version: 2.1
 Name: goto_conversion
-Version: 0.2.0
-Summary: Novel Conversion of Betting Odds to Probabilities
+Version: 0.3.0
+Summary: Gambling Odds To Outcome probabilities Conversion (goto_conversion)
 Author: Kaito Goto
 Project-URL: Homepage, https://github.com/gotoConversion/goto_conversion
 Project-URL: Bug Tracker, https://github.com/gotoConversion/goto_conversion/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# goto_conversion: Novel Conversion of Betting Odds to Probabilities
+# Gambling Odds To Outcome probabilities Conversion (goto_conversion)
 
 The most common method used to convert betting odds to probabilities is to normalise the inverse odds (Multiplicative conversion). However, this method does not consider the favourite-longshot bias. 
 
 To the best of our knowledge, there are two existing methods that attempt to consider the favourite-longshot bias. (i) Shin conversion [[1](#1),[2](#2),[3](#3)] maximises the expected profit for the bookmakers assuming a small proportion of bettors have inside information. (ii) Power conversion [[4](#4)] raises all inverse odds to the same constant power. However, both of these methods require iterative computation to convert betting odds to probabilities.
 
-Our proposed method (`goto_conversion`) is significantly more efficient than Shin and Power conversion because it converts betting odds to probabilities directly without iterative computation.
+Our proposed method, **G**ambling **O**dds **T**o **O**utcome probabilities **Conversion** (`goto_conversion`) is significantly more efficient than Shin and Power conversion because it converts betting odds to probabilities directly without iterative computation.
 
 The `goto_conversion` reduces all inverse odds by the same units of standard error. This attempts to consider the favourite-longshot bias by utilising the proportionately wider standard errors implied for inverses of longshot odds and vice-versa.
 
 Furthermore, our tables of experiment results show that the `goto_conversion` converts betting odds to probabilities more accurately than all three of these existing methods.
 
 The favourite-longshot bias is not limited to gambling markets, it exists in stock markets too. Thus, we applied the original `goto_conversion` to stock markets by defining the `zero_sum` variant. Under the same philosophy as the original `goto_conversion`, `zero_sum` adjusts all predicted stock prices (e.g. weighted average price) by the same units of standard error to ensure all predicted stock prices relative to the index price (e.g. weighted average nasdaq price) sum to zero. This attempts to consider the favourite-longshot bias by utilising the wider standard errors implied for predicted stock prices with low trade volume and vice-versa.
 
 # Citations (not limited to, unofficial)
 
-[Most Voted Public Solution from 2024 Optiver Kaggle Competition](https://www.kaggle.com/code/ravi20076/optiver-baseline-models?scriptVersionId=152991375)
+[Most Voted Solution from 2023 Optiver Kaggle Competition](https://www.kaggle.com/code/ravi20076/optiver-baseline-models?scriptVersionId=152991375)
 
-[1xGold and 2xSilver Medal Winning Public Solution from 2019 to 2022 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/1xgold-2xsilvers-key-ingredient)
+[Gold Medal Winning (14th out of 3225) Solution from 2023 Optiver Kaggle Competition (the `zero_sum` variant)](https://www.kaggle.com/competitions/optiver-trading-at-the-close/discussion/462653)
 
-[Bronze Medal Winning Public Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/updated-1xgold-2xsilvers-key-ingredient)
+[Gold Medal Winning (3rd out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/495101)
+
+[Gold Medal Winning (4th out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/competitions/march-machine-learning-mania-2024/discussion/494407)
+
+[1xGold and 2xSilver Medal Winning Solution from 2019 to 2022 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/1xgold-2xsilvers-key-ingredient)
+
+[15xBronze Medal Winning (86th to 100th place out of 821) Solution from 2024 March Mania Kaggle Competition](https://www.kaggle.com/code/kaito510/updated-1xgold-2xsilvers-key-ingredient)
 
 # Installation
 
 Requires Python 3.7 or above.
 
 ```
 pip install goto-conversion
@@ -68,26 +74,24 @@
 
 # Pseudo Code
 
 ![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/PseudoCode.png?raw=true)
 
 # Experiment Results
 
-The experiment results table directly below is based on the same 6,000 football matches' betting odds (home win, draw or away win) across four different bookmakers.
+Brier Score was mainly used to evaluate the accuracy of the probabilities implied by each conversion method. The Brier Score is essentially the mean squared error of the probabilities relative to the ground truth. Ranked Probability Score (RPS) was additionally used to evaluate the probabilities for football betting odds because the outcome is ordinal (home win, draw and away win). RPS is essentially the Brier Score on the cumulative probabilities.
 
-![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/FballExperiment.png?raw=true)
+The experiment results table directly below is based on the same 6,000 football matches' betting odds (home win, draw or away win) across four different bookmakers. `goto_conversion` outperforms all other conversion methods for all four bookmakers. Kaggle notebook to reproduce the table directly below can be found [here](https://www.kaggle.com/code/kaito510/novel-conversion-of-football-betting-odds).
 
-Kaggle notebook to reproduce the table directly above: https://www.kaggle.com/code/kaito510/novel-conversion-of-football-betting-odds
+![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/FballExperiment.png?raw=true)
 
-The experiment results table directly below is based on 6,348 horse races' betting odds for the win and place markets.
+The experiment results table directly below is based on 6,348 horse races' betting odds for the win and place markets. `goto_conversion` outperforms all other conversion methods for both win and place betting markets. Kaggle notebook to reproduce the table directly below can be found [here](https://www.kaggle.com/code/kaito510/novel-conversion-of-horse-racing-odds).
 
 ![alt text](https://github.com/gotoConversion/goto_conversion/blob/main/RacingExperiment.png?raw=true)
 
-Kaggle notebook to reproduce the table directly above: https://www.kaggle.com/code/kaito510/novel-conversion-of-horse-racing-odds
-
 # References
 
 <a id="1">[1]</a> 
 [H. S. Shin, “Prices of State Contingent Claims with Insider
 traders, and the Favorite-Longshot Bias”. The Economic
 Journal, 1992, 102, pp. 426-435.](https://doi.org/10.2307/2234526)
```

