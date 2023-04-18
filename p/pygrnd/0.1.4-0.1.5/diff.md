# Comparing `tmp/pygrnd-0.1.4.tar.gz` & `tmp/pygrnd-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrnd-0.1.4.tar", last modified: Mon Mar  6 16:15:49 2023, max compression
+gzip compressed data, was "pygrnd-0.1.5.tar", last modified: Tue Apr 18 06:44:05 2023, max compression
```

## Comparing `pygrnd-0.1.4.tar` & `pygrnd-0.1.5.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:15:49.093193 pygrnd-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-03-06 16:15:35.000000 pygrnd-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-03-06 16:15:49.093193 pygrnd-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-03-06 16:15:35.000000 pygrnd-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:15:49.089193 pygrnd-0.1.4/pygrnd/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:15:49.089193 pygrnd-0.1.4/pygrnd/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/optimize/MonteCarloSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    55703 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/optimize/UCPquboFunctionLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/optimize/bruteforce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/optimize/meritorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15040 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/optimize/qaoa.py
--rw-r--r--   0 runner    (1001) docker     (123)    39791 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/optimize/sat_ucp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:15:49.089193 pygrnd-0.1.4/pygrnd/qc/
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/qc/MaximumLikelihoodForQAEwoPE.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/qc/QAE.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24444 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/qc/brm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/qc/brm_oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/qc/brm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/qc/circuitConstructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/qc/circuitConstructor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/qc/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/qc/lowDepthQAEgradientDescent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/qc/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18162 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/qc/parallelQAE.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/qc/patternGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21171 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/qc/patternReducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/qc/probabilisticNetworks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16149 2023-03-06 16:15:35.000000 pygrnd-0.1.4/pygrnd/qc/qml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:15:49.089193 pygrnd-0.1.4/pygrnd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-03-06 16:15:49.000000 pygrnd-0.1.4/pygrnd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-06 16:15:49.000000 pygrnd-0.1.4/pygrnd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 16:15:49.000000 pygrnd-0.1.4/pygrnd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 16:15:48.000000 pygrnd-0.1.4/pygrnd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-06 16:15:49.000000 pygrnd-0.1.4/pygrnd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-06 16:15:49.000000 pygrnd-0.1.4/pygrnd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 16:15:49.093193 pygrnd-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-03-06 16:15:35.000000 pygrnd-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:05.736500 pygrnd-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-18 06:43:56.000000 pygrnd-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-04-18 06:44:05.736500 pygrnd-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-04-18 06:43:56.000000 pygrnd-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:05.732500 pygrnd-0.1.5/pygrnd/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:05.732500 pygrnd-0.1.5/pygrnd/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/optimize/MonteCarloSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56649 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/optimize/UCPquboFunctionLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/optimize/bruteforce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/optimize/meritorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15040 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/optimize/qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27489 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/optimize/qmco.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39791 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/optimize/sat_ucp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:05.736500 pygrnd-0.1.5/pygrnd/qc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/MaximumLikelihoodForQAEwoPE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/QAE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24444 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/brm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/brm_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/brm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/circuitConstructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/circuitConstructor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/lowDepthQAEgradientDescent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18162 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/parallelQAE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/patternGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21171 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/patternReducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/probabilisticNetworks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/qml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:05.732500 pygrnd-0.1.5/pygrnd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-04-18 06:44:05.000000 pygrnd-0.1.5/pygrnd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-18 06:44:05.000000 pygrnd-0.1.5/pygrnd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:44:05.000000 pygrnd-0.1.5/pygrnd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:44:05.000000 pygrnd-0.1.5/pygrnd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-18 06:44:05.000000 pygrnd-0.1.5/pygrnd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 06:44:05.000000 pygrnd-0.1.5/pygrnd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 06:44:05.736500 pygrnd-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-18 06:43:56.000000 pygrnd-0.1.5/setup.py
```

### Comparing `pygrnd-0.1.4/LICENSE` & `pygrnd-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/PKG-INFO` & `pygrnd-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pygrnd
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python library for quantum algorithms and software
 Home-page: https://github.com/JoSQUANTUM/pygrnd
 Author: JoS QUANTUM
 Author-email: contact@jos-quantum.de
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pygrnd 
-is a libary of various quantum algorithms written by the Team JoS QUANTUM GmbH to support the development of Applications for quantum computing in Finance, Insurance and Energy. The framework is a collection of open source libraries that enables building quantum models and prototypes and usage of our quantum algorithms.
+is a library of various quantum algorithms written by the Team JoS QUANTUM GmbH to support the development of Applications for quantum computing in Finance, Insurance and Energy. The framework is a collection of open source libraries that enables building quantum models and prototypes and usage of our quantum algorithms.
 
 pygrnd depends on different modules: 
 
     Quantum machine learning: pennylane (pennylane.ai/)
     Monte Carlo simulation: qiskit (qiskit.org)
     Optimization: qiskit, dimod (docs.ocean.dwavesys.com/en/stable/)
 
@@ -29,24 +29,27 @@
    
     pip install qiskit
     pip install numpy
     pip install dimod
     pip install dwave-greedy
     pip install pennylane
  
-# Tutorials
+# Tutorials and notebooks
+
+You can find example notebooks with usage of pygrnd functions in ``notebooks/``
 
 ## Quantum Risk Modelling
 
-Workflow to define a risk model like outlined in (https://arxiv.org/abs/2103.05475).
+Notebook: ``risk_model.ipynb`` and ``sensitivity_analysis.ipynb``
+
+Workflow to define a risk model like outlined in (<https://arxiv.org/abs/2103.05475>).
 Build a Grover operator with a state for which the overall probabilty should be evaluated.
 Standard Quantum Amplitude Estimation algorithm.
 Using QASM simulator you should not use more than 20 qubits (including the QAEqubits) on your local machine using simulator.
 
-
     - Input risk items, instrinsic and transition probabilities
     - List of states to estimate probabilities for the desired state
     - Precision for the QAE
     - Number of shots
 
 
 ### Syntax
@@ -108,14 +111,19 @@
 
     states, summe = modelProbabilities(nodes,edges,probsNodes,probsEdges)
     probsMonteCarlo = evaluateRiskModelMonteCarlo(nodes, edges, probsNodes, probsEdges, rounds)
 
 
 ## Amplitude Estimation without Phase Estimation
 
+Notebook: ``parallelQAE.ipynb``
+
+This notebook explaines functions for our proprietary quantum algorithm described in <https://arxiv.org/abs/2204.01337>.
+Parallel QAE is a quantum algorithm for Monte Carlo simulation on quantum computers with reduced gate depth and therefore a candidate to run quantum models on noisy quantum computers without full error-correction.
+
 - We have an operator A and a set of good results that have probability a in total.
 - We construct the Grover oracle G for A.
 - We construct a circuit with m calls of G in addition to one call of A and we run the circuit N times. We obtain h good results.
 - For different values of m we repeat this procedure.
 - We obtain vectors vectorN, vectorM and vectorH.
 - Use these parameters to guess the value a with maximum likelihood method.
 - The method uses a gradient descent with a random starting point and a stepSize=0.01 as default step size.
@@ -129,15 +137,19 @@
     vectorH = [21, 1, 29]
     bestTheta,bestProb = loopGradientOptimizerVector(vectorN, vectorM, vectorH, rounds=10, stepSize=0.01)
     print("best guess theta=",bestTheta)
     print("best guess prob=",bestProb)
 
 
 
-## Pattern-based Circuit optimizer
+## Pattern-based circuit optimizer
+
+Notebook: ``circuitConstructor.ipynb``
+
+The methods demonstrate how quantum circuits can be optimized to reduced gate depth. The methods are implementations or variations of algorithms of the following paper <https://doi.org/10.1103/PhysRevA.52.3457>. 
 
 ### Background: Patterns
 
 A pattern is an abstract representation of a sequence of quantum gates that corresponds to the identity. The gates are denoted by a string, e.g. H or X, and the parameters are variables or concrete values. The gates act on qubits that are denoted by numbers only.
 
 An example for a pattern:
 
@@ -204,29 +216,41 @@
 ## Quantum machine learing
 
 Quantum machine learning functions for regression and classifiction. 
 
 
 ### Example: Classification
 
-In ``notebooks/outlier_detection.ipynb`` an example for fraud detection (binary classification) based on a publicly available Kaggle data set is done.
+Notebook: ``notebooks/outlier_detection.ipynb`` 
+
+Example for fraud detection (binary classification) using parametrized quantum circuits to analyze a publicly available Kaggle data set.
 
 
 ### Example: Forecasting (coming soon)
 
 
 ### Example: Synthetic data (coming soon)
 
 
-
 ## Optimization
 
+
+
+Notebook ``ucp_relaxedQUBO.ipynb`` explaines the main idea of how to encode several variations of the Unit Commitment Problem (UCP, <https://en.wikipedia.org/wiki/Unit_commitment_problem_in_electrical_power_production>) as a QUBO (quadratic unconstrained binary optimization). 
+The UCP answers the following question: Which power generator should run at what level at which time to satisfy constrains like demand in each time step, power generator parameter like minimum and maximum up and down times and ramps. Because of growing amount of renewable energy grid in-feed, uncertainty of changing weather conditions requires fast precise solutions to the UCP. The notebook explains how the approach can be seen as a first attempt towards robust optimization by incorporating uncertainty from renewable energy supply. <https://arxiv.org/abs/2301.01108>
+
 Implementations of different QUBO (Quadratic Unconstrained Binary Optimization) solver for benchmarks.
 Methods for QUBO construction and solving. Classical brute-force solver, Monte Carlo, Quantum annealing (D-Wave), simulated annealing, Quantum approximate optimization algorithm.
 
+Notebook ``ucp_sat.ipynb`` explaines how to encode constraints as SAT formulation. THis construction is then mapped to a QUBO and several problem sets are benchmarked.
+
+Notebook ``merit_order.ipynb`` is the very first version of the merit order problem with power generator costs, static supply and demand formulated as knapsack.
+
+This work is based on the governmental funded project "EnerQuant":
+<https://ercim-news.ercim.eu/en128/special/energy-economics-fundamental-modelling-with-quantum-algorithms>
 
 ### Monte Carlo random search
 
 - randomly generate solution vector
 - calculation of matrix product x^T Q x
 - iterate N times
 
@@ -276,14 +300,16 @@
     Q = np.array([[10,-3,-4,-6],[-3,4,-2,-3],[-4,-2,6,-5],[-6,-3,-5,12]])
     N=10
     r,a=MCgradientSearch(Q,10)
     print(r,a)
 
 ### Quantum Approximate Optimization Algorithm (QAOA)
 
+A quantum algorithm to solve QUBO formulations on gate-based quantum computers. The function requires qiskit to construct circuits (qiskit high-level functions are not used).
+
 - input QUBO matrix as numpy array
 - build cost Hamiltonian U(gamma) using mapping x --> (x - 1) /2 (matrixConvertInv(m))
 - build mixer Hamiltonian U(beta)
 - construct one layer circuit with initial random beta, gamma values
 - execute on backend (default: Aer.get_backend('qasm_simulator'))
 - derive max count
 - calculate expectation value
```

### Comparing `pygrnd-0.1.4/README.md` & `pygrnd-0.1.5/pygrnd.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,23 @@
+Metadata-Version: 2.1
+Name: pygrnd
+Version: 0.1.5
+Summary: A python library for quantum algorithms and software
+Home-page: https://github.com/JoSQUANTUM/pygrnd
+Author: JoS QUANTUM
+Author-email: contact@jos-quantum.de
+License: Apache 2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pygrnd 
-is a libary of various quantum algorithms written by the Team JoS QUANTUM GmbH to support the development of Applications for quantum computing in Finance, Insurance and Energy. The framework is a collection of open source libraries that enables building quantum models and prototypes and usage of our quantum algorithms.
+is a library of various quantum algorithms written by the Team JoS QUANTUM GmbH to support the development of Applications for quantum computing in Finance, Insurance and Energy. The framework is a collection of open source libraries that enables building quantum models and prototypes and usage of our quantum algorithms.
 
 pygrnd depends on different modules: 
 
     Quantum machine learning: pennylane (pennylane.ai/)
     Monte Carlo simulation: qiskit (qiskit.org)
     Optimization: qiskit, dimod (docs.ocean.dwavesys.com/en/stable/)
 
@@ -15,24 +29,27 @@
    
     pip install qiskit
     pip install numpy
     pip install dimod
     pip install dwave-greedy
     pip install pennylane
  
-# Tutorials
+# Tutorials and notebooks
+
+You can find example notebooks with usage of pygrnd functions in ``notebooks/``
 
 ## Quantum Risk Modelling
 
-Workflow to define a risk model like outlined in (https://arxiv.org/abs/2103.05475).
+Notebook: ``risk_model.ipynb`` and ``sensitivity_analysis.ipynb``
+
+Workflow to define a risk model like outlined in (<https://arxiv.org/abs/2103.05475>).
 Build a Grover operator with a state for which the overall probabilty should be evaluated.
 Standard Quantum Amplitude Estimation algorithm.
 Using QASM simulator you should not use more than 20 qubits (including the QAEqubits) on your local machine using simulator.
 
-
     - Input risk items, instrinsic and transition probabilities
     - List of states to estimate probabilities for the desired state
     - Precision for the QAE
     - Number of shots
 
 
 ### Syntax
@@ -94,14 +111,19 @@
 
     states, summe = modelProbabilities(nodes,edges,probsNodes,probsEdges)
     probsMonteCarlo = evaluateRiskModelMonteCarlo(nodes, edges, probsNodes, probsEdges, rounds)
 
 
 ## Amplitude Estimation without Phase Estimation
 
+Notebook: ``parallelQAE.ipynb``
+
+This notebook explaines functions for our proprietary quantum algorithm described in <https://arxiv.org/abs/2204.01337>.
+Parallel QAE is a quantum algorithm for Monte Carlo simulation on quantum computers with reduced gate depth and therefore a candidate to run quantum models on noisy quantum computers without full error-correction.
+
 - We have an operator A and a set of good results that have probability a in total.
 - We construct the Grover oracle G for A.
 - We construct a circuit with m calls of G in addition to one call of A and we run the circuit N times. We obtain h good results.
 - For different values of m we repeat this procedure.
 - We obtain vectors vectorN, vectorM and vectorH.
 - Use these parameters to guess the value a with maximum likelihood method.
 - The method uses a gradient descent with a random starting point and a stepSize=0.01 as default step size.
@@ -115,15 +137,19 @@
     vectorH = [21, 1, 29]
     bestTheta,bestProb = loopGradientOptimizerVector(vectorN, vectorM, vectorH, rounds=10, stepSize=0.01)
     print("best guess theta=",bestTheta)
     print("best guess prob=",bestProb)
 
 
 
-## Pattern-based Circuit optimizer
+## Pattern-based circuit optimizer
+
+Notebook: ``circuitConstructor.ipynb``
+
+The methods demonstrate how quantum circuits can be optimized to reduced gate depth. The methods are implementations or variations of algorithms of the following paper <https://doi.org/10.1103/PhysRevA.52.3457>. 
 
 ### Background: Patterns
 
 A pattern is an abstract representation of a sequence of quantum gates that corresponds to the identity. The gates are denoted by a string, e.g. H or X, and the parameters are variables or concrete values. The gates act on qubits that are denoted by numbers only.
 
 An example for a pattern:
 
@@ -190,29 +216,41 @@
 ## Quantum machine learing
 
 Quantum machine learning functions for regression and classifiction. 
 
 
 ### Example: Classification
 
-In ``notebooks/outlier_detection.ipynb`` an example for fraud detection (binary classification) based on a publicly available Kaggle data set is done.
+Notebook: ``notebooks/outlier_detection.ipynb`` 
+
+Example for fraud detection (binary classification) using parametrized quantum circuits to analyze a publicly available Kaggle data set.
 
 
 ### Example: Forecasting (coming soon)
 
 
 ### Example: Synthetic data (coming soon)
 
 
-
 ## Optimization
 
+
+
+Notebook ``ucp_relaxedQUBO.ipynb`` explaines the main idea of how to encode several variations of the Unit Commitment Problem (UCP, <https://en.wikipedia.org/wiki/Unit_commitment_problem_in_electrical_power_production>) as a QUBO (quadratic unconstrained binary optimization). 
+The UCP answers the following question: Which power generator should run at what level at which time to satisfy constrains like demand in each time step, power generator parameter like minimum and maximum up and down times and ramps. Because of growing amount of renewable energy grid in-feed, uncertainty of changing weather conditions requires fast precise solutions to the UCP. The notebook explains how the approach can be seen as a first attempt towards robust optimization by incorporating uncertainty from renewable energy supply. <https://arxiv.org/abs/2301.01108>
+
 Implementations of different QUBO (Quadratic Unconstrained Binary Optimization) solver for benchmarks.
 Methods for QUBO construction and solving. Classical brute-force solver, Monte Carlo, Quantum annealing (D-Wave), simulated annealing, Quantum approximate optimization algorithm.
 
+Notebook ``ucp_sat.ipynb`` explaines how to encode constraints as SAT formulation. THis construction is then mapped to a QUBO and several problem sets are benchmarked.
+
+Notebook ``merit_order.ipynb`` is the very first version of the merit order problem with power generator costs, static supply and demand formulated as knapsack.
+
+This work is based on the governmental funded project "EnerQuant":
+<https://ercim-news.ercim.eu/en128/special/energy-economics-fundamental-modelling-with-quantum-algorithms>
 
 ### Monte Carlo random search
 
 - randomly generate solution vector
 - calculation of matrix product x^T Q x
 - iterate N times
 
@@ -262,14 +300,16 @@
     Q = np.array([[10,-3,-4,-6],[-3,4,-2,-3],[-4,-2,6,-5],[-6,-3,-5,12]])
     N=10
     r,a=MCgradientSearch(Q,10)
     print(r,a)
 
 ### Quantum Approximate Optimization Algorithm (QAOA)
 
+A quantum algorithm to solve QUBO formulations on gate-based quantum computers. The function requires qiskit to construct circuits (qiskit high-level functions are not used).
+
 - input QUBO matrix as numpy array
 - build cost Hamiltonian U(gamma) using mapping x --> (x - 1) /2 (matrixConvertInv(m))
 - build mixer Hamiltonian U(beta)
 - construct one layer circuit with initial random beta, gamma values
 - execute on backend (default: Aer.get_backend('qasm_simulator'))
 - derive max count
 - calculate expectation value
```

### Comparing `pygrnd-0.1.4/pygrnd/__init__.py` & `pygrnd-0.1.5/pygrnd/__init__.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/optimize/MonteCarloSolver.py` & `pygrnd-0.1.5/pygrnd/optimize/MonteCarloSolver.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/optimize/UCPquboFunctionLibrary.py` & `pygrnd-0.1.5/pygrnd/optimize/UCPquboFunctionLibrary.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,16 @@
 import pandas as pd
 import seaborn as sns
 import time
 import dimod
 import neal
 import greedy
 
-from azure.quantum.optimization import Problem, ProblemType, Term
-from azure.quantum import Workspace
 
-
-def penaltycheck(p,dgen,mingen,start,minup,mindown,on,T,n,pres):
+def penaltycheck(p,dgen,mingen,start,minup,mindown,on,T,n,pres,verbose=False):
     
     """
     function penaltycheck checks if constraints are violated by checking the binary solution-vector "p"
     """
     
     pmincheck=True
     oncheck=True
@@ -79,22 +76,29 @@
                     if t+mindown[i]>T:
                         enddown=T
                     else:
                         enddown=t+mindown[i]
                     for tau in range(t,enddown):
                         if power[tau][i]>0:
                             mindowncheck=False
-    print('pmincheck: ',pmincheck)
-    print('minupcheck: ',minupcheck)
-    print('mindowncheck: ',mindowncheck)
-    print('oncheck: ',oncheck)
-    print('startcheck: ',startcheck)
+    
+    if verbose==True:
+        print('pmincheck: ',pmincheck)
+        print('minupcheck: ',minupcheck)
+        print('mindowncheck: ',mindowncheck)
+        print('oncheck: ',oncheck)
+        print('startcheck: ',startcheck)
+    
     if pmincheck==False or minupcheck==False or mindowncheck==False or oncheck==False or startcheck==False:
         okay=False
     quality=1-(minupviolation+mingenviolation)/(n*T)
+    
+    if verbose==True:
+        print('all checks: ',okay)
+    
     return okay, pmincheck, oncheck, startcheck, minupcheck, mindowncheck, quality
 
 
 def costsummation(p,dgen,mingen,varcost,startcost,T,n,pres): 
 
     """
     function to calculate the costs from a binary solution vector "p"  #dgen hold the discretized power stages of the units
@@ -128,14 +132,16 @@
 def BruteForceUCPqubo(M,dgen,varcost,startcost,mingen,minup,mindown,T,n,pres,bestprice, bestpriceAns, bestobjective, bestobjectiveAns, bestobjectiveprice, bestpriceobj, boolcheck,graphicsout):
 
     """
     Solve QUBO brute force by iterating through every possible 2^N combinations of the solution vector x^T Q x and checking the objective
 
     """
 
+    print("Start solver engine: Brute force iterations (very inefficient and can be very long running)")
+
     starttime = time.process_time()
     m=len(M)                                                                                      #check all possible combinations for solution vector and search global minimum
     nonzeros=0
     for i in range(m):
         for j in range(m):
             if abs(M[i,j])>0.01:
                 nonzeros=nonzeros+1
@@ -191,37 +197,40 @@
                     bestpriceobj=r
             minimum_value=res
             minimum_vector=np.array(v[0]).flatten()
         combiobjpriceokay=[res,price,errorquality]
         combined.append(np.array(combiobjpriceokay))
     timetosolve=time.process_time() - starttime                                               # calculate time for problem saving
     if graphicsout==True:
-        print('time to brute solve the best solution:',timetosolve)
-
+        
         fig1, ax1 = plt.subplots()                                                            # plot energy landscape and costs of all possible solutions
 
         ax2 = ax1.twinx()
         ax1.plot([k for k in range(len(saveresultsobjective))],[saveresultsobjective[k][0] for k in range(len(saveresultsobjective))],'b-')
         ax2.plot([k for k in range(len(saveresultsprice))],[saveresultsprice[k][0] for k in range(len(saveresultsprice))],'rx')
 
         ax1.set_xlabel('states', fontsize=20)
         ax1.set_ylabel('objective value', color='b', fontsize=20)
         ax2.set_ylabel('cost value', color='r', fontsize=20)
         plt.show()
 
+    print("Time to solve (wall time): ", timetosolve)
+
     return minimum_value, minimum_vector, combined, saveresultsprice, saveresultsobjective, errors, bestprice, bestpriceAns, bestobjective, bestobjectiveAns, bestobjectiveprice, bestpriceobj, timetosolve
 
 
 
 
 def MonteCarloUCPqubo(Q,N,dgen,varcost,startcost,mingen,minup,mindown,T,n,pres,bestprice, bestpriceAns, bestobjective, bestobjectiveAns, bestobjectiveprice, bestpriceobj, boolcheck,graphicsout):
 
     """
     Monte Carlo solver that randomly samples from solution space N times a given number of binary vectors and checks if constraints are fulfilled
     """
+    print("Start solver engine: Monte Carlo random")
+    print(Num, "iterations")  
 
     starttime = time.process_time()
     m=len(Q)
     nonzeros=0
     saveresultsprice=[]
     saveresultsobjective=[]
     errors=[]
@@ -283,36 +292,39 @@
             a=v[0]
 
         combiobjpriceokay=[r,price,errorquality]
         combined.append(np.array(combiobjpriceokay))
 
     timetosolve=time.process_time() - starttime                                               # calculate time for problem saving
     if graphicsout==True:
-        print('time to brute solve the best solution:',timetosolve)
-
         fig1, ax1 = plt.subplots()                                                # plot energy landscape and costs of all possible solutions
 
         ax2 = ax1.twinx()
         ax1.plot([k for k in range(len(saveresultsobjective))],[saveresultsobjective[k][0] for k in range(len(saveresultsobjective))],'b-')
         ax2.plot([k for k in range(len(saveresultsprice))],[saveresultsprice[k][0] for k in range(len(saveresultsprice))],'rx')
 
         ax1.set_xlabel('states', fontsize=20)
         ax1.set_ylabel('objective value', color='b', fontsize=20)
         ax2.set_ylabel('cost value', color='r', fontsize=20)
         plt.show()
 
+    print("Time to solve (wall time): ", timetosolve)
+    
     return cheapestPrice , a, combined, errors, bestprice, bestpriceAns, bestpriceobj, bestobjectiveprice, bestobjectiveAns, bestobjective, timetosolve
 
 
 def MCsteepestdescentUCPqubo(Q,N,dgen,varcost,startcost,mingen,minup,mindown,T,n,pres,bestprice, bestpriceAns, bestobjective, bestobjectiveAns, bestobjectiveprice, bestpriceobj, boolcheck,graphicsout):
 
     """
     Variant of the Monte Carlo solver
     """
 
+    print("Start solver engine: Monte Carlo steepest descent")
+    print(rounds,"rounds and ",Num, "iterations")
+
     starttime = time.process_time()
     v=np.random.randint(2, size=(1, len(Q)))
 
     result=[]
     current=Q[0][0]
     counter=0
     for m in Q:
@@ -409,40 +421,41 @@
             a=v[0]
 
         combiobjpriceokay=[r,price,errorquality]
         combined.append(np.array(combiobjpriceokay))
 
     timetosolve=time.process_time() - starttime                                               # calculate time for problem saving
     if graphicsout==True:
-        print('time to brute solve the best solution:',timetosolve)
-
         fig1, ax1 = plt.subplots()
-
         ax2 = ax1.twinx()
         ax1.plot([k for k in range(len(saveresultsobjective))],[saveresultsobjective[k][0] for k in range(len(saveresultsobjective))],'b-')
         ax2.plot([k for k in range(len(saveresultsprice))],[saveresultsprice[k][0] for k in range(len(saveresultsprice))],'rx')
-
         ax1.set_xlabel('states', fontsize=20)
         ax1.set_ylabel('objective value', color='b', fontsize=20)
         ax2.set_ylabel('cost value', color='r', fontsize=20)
         plt.show()
 
+    print("Time to solve (wall time): ",timetosolve)
+
     return r, a, combined, errors, bestprice, bestpriceAns, bestpriceobj, bestobjectiveprice, bestobjectiveAns, bestobjective, timetosolve
 
 
 
 def SimulatedAnnealingUCPqubo(Q,Num,rounds,dgen,varcost,startcost,mingen,minup,mindown,T,n,pres,bestprice, bestpriceAns, bestobjective, bestobjectiveAns, bestobjectiveprice, bestpriceobj, boolcheck, Qcost,graphicsout):
     
     """
     Simulated annealing solver using D-Waves "neal" package
     Q: Qubo martix as input
     Num: Number of samples
     rounds: number of subsequent rounds of simulated annealing with initial solutions as input states
     """
 
+    print("Start solver engine: Simulated annealing")
+    print(rounds,"rounds and ",Num, "iterations")
+
     import dimod
     import neal
     import greedy
     import time
 
     q=Q
     qubo={}
@@ -517,14 +530,15 @@
             if price<bestprice:  # find best solution with lowest costs
                 bestprice=price
                 bestpriceAns=solv[L]
                 bestpriceobj=solobj[L]
         combiobjpriceokay=[solobj[L],np.array(price),np.array(errorquality)]
         combined.append(np.array(combiobjpriceokay))
 
+    print("Time to solve (wall time): ",timetosolve)
 
     return price, Ans, combined, errors, bestprice, bestpriceAns, bestpriceobj, bestobjectiveprice, bestobjectiveAns, bestobjective, timetosolve
 
 
 
 
 def QuantumAnnealingUCPqubo(Q,Num,rounds,DWtoken,dgen,varcost,startcost,mingen,minup,mindown,T,n,pres,bestprice, bestpriceAns, bestobjective, bestobjectiveAns, bestobjectiveprice, bestpriceobj, boolcheck, Qcost, graphicsout):
@@ -532,14 +546,17 @@
     """
     Solver that uses quantum annealing machines from D-Wave to calculate a solution
     Q: Qubo martix as input
     Num: Number of samples
     rounds: number of subsequent rounds of simulated annealing with initial solutions as input states
     """
 
+    print("Start solver engine: D-Wave QPU quantum annealing")
+    print(Num, "iterations, ","rounds",rounds)
+
     import dimod
     import neal
     import greedy
     import time
 
     from dwave.system import LeapHybridSampler
     from dimod import Binary, ConstrainedQuadraticModel, quicksum
@@ -638,21 +655,29 @@
             if price<bestprice:                                                                             # find best solution with lowest costs
                 bestprice=price
                 bestpriceAns=solv[L]
                 bestpriceobj=solobj[L]
         combiobjpriceokay=[solobj[L],np.array(price),np.array(errorquality)]
         combined.append(combiobjpriceokay)
 
+    print("Time to solve (wall time): ",timetosolve)
+
     return price, Ans, combined, errors, bestprice, bestpriceAns, bestpriceobj, bestobjectiveprice, bestobjectiveAns, bestobjective, timetosolve
 
+## Uncomment to use Azure QIO
+"""
 def OptProblem(CostMatrix) -> Problem:
 
-    """
+    # Uncomment to use Azure Quantum-Inspired Optimization
+    #from azure.quantum.optimization import Problem, ProblemType, Term
+    #from azure.quantum import Workspace
+
+    """"""
     Azure routine to load matrix to Problem
-    """
+    """"""
 
     terms = []
 
     for i in range(0, len(CostMatrix)): 
         for j in range(0, len(CostMatrix)): 
 
             terms.append(
@@ -664,22 +689,22 @@
 
 
     return Problem(name="ucp", problem_type=ProblemType.pubo, terms=terms)
 
 
 def AzureRoutinePT(workspace,Q,Num,dgen,varcost,startcost,mingen,minup,mindown,T,n,pres,bestprice, bestpriceAns, bestobjective, bestobjectiveAns, bestobjectiveprice, bestpriceobj, boolcheck, Qcost,graphicsout):
 
-    """
+    """"""
     Microsoft Quantum Inspired Optimization
     Azure quantum-inspired algorithms: Parallel Tempering
     Rephrases the optimization problem as a thermodynamic system and runs multiple copies of a system, randomly initialized, at different temperatures. Then, based on a specific protocol, exchanges configurations at different temperatures to find the optimal configuration.
     Azure workspace need to be loaded
     Q: Qubo martix as input
     Num: Number of samples
-    """
+    """"""
 
     from azure.quantum.optimization import Problem, ProblemType, Term
     from azure.quantum.optimization import ParallelTempering
     
     solver_ = ParallelTempering(workspace)
     Qproblem=OptProblem(Q)
 
@@ -758,22 +783,22 @@
         combiobjpriceokay=[solobj[L],price,errorquality]
         combined5.append(combiobjpriceokay)
 
     return price5, Ans, combined5, errors5, bestprice, bestpriceAns, bestobjective, bestobjectiveAns, bestobjectiveprice, bestpriceobj, timetosolve
 
 def AzureRoutineQMC(workspace,Q,Num,dgen,varcost,startcost,mingen,minup,mindown,T,n,pres,bestprice, bestpriceAns, bestobjective, bestobjectiveAns, bestobjectiveprice, bestpriceobj, boolcheck, Qcost,graphicsout):
 
-    """
+    """"""
     Microsoft Quantum Inspired Optimization
     Azure quantum-inspired algorithms: Quantum Monte Carlo
     Similar to Simulated Annealing but the changes are by simulating quantum-tunneling through barriers rather than using thermal energy jumps.
     Azure workspace need to be loaded
     Q: Qubo martix as input
     Num: Number of samples
-    """
+    """"""
     
     from azure.quantum.optimization import Problem, ProblemType, Term
     from azure.quantum.optimization import QuantumMonteCarlo
     
     solver_ = QuantumMonteCarlo(workspace)
     Qproblem=OptProblem(Q)
     starttime = time.process_time()
@@ -849,22 +874,22 @@
         combiobjpriceokay=[solobj[L],price,errorquality]
         combined6.append(combiobjpriceokay)
 
     return price6, Ans, combined6, errors6, bestprice, bestpriceAns, bestobjective, bestobjectiveAns, bestobjectiveprice, bestpriceobj, timetosolve
 
 def AzureRoutineSQMC(workspace,Q,Num,dgen,varcost,startcost,mingen,minup,mindown,T,n,pres,bestprice, bestpriceAns, bestobjective, bestobjectiveAns, bestobjectiveprice, bestpriceobj, boolcheck, Qcost,graphicsout):
 
-    """
+    """"""
     Microsoft Quantum Inspired Optimization
     Azure quantum-inspired algorithms: Substochastic Monte Carlo
     Substochastic Monte Carlo is a diffusion Monte Carlo algorithm inspired by adiabatic quantum computation. It simulates the diffusion of a population of walkers in search space, while walkers are removed or duplicated based on how they perform according to the cost function.
     Azure workspace need to be loaded
     Q: Qubo martix as input
     Num: Number of samples
-    """
+    """"""
     
     from azure.quantum.optimization import Problem, ProblemType, Term
     from azure.quantum.optimization import SubstochasticMonteCarlo
 
     solver_ = SubstochasticMonteCarlo(workspace, seed=48, timeout=10)(workspace)
     Qproblem=OptProblem(Q)
     starttime = time.process_time()
@@ -937,24 +962,29 @@
                 bestpriceAns=solv[L]
                 bestpriceobj=solobj[L]
         combiobjpriceokay=[solobj[L],price,errorquality]
         combined7.append(combiobjpriceokay)
 
     return price7, Ans, combined7, errors7, bestprice, bestpriceAns, bestobjective, bestobjectiveAns, bestobjectiveprice, bestpriceobj, timetosolve
 
+"""
+
+
 def buildUCPqubo(autoset,n,pres,T,d,dgen,Clist,varcost,startcost,minup,mindown,mingen,maxgen):
 
     """
     Build the QUBO for the unit commitment problem as outlined in the following paper:
     M.C. Braun, T. Decker, N. Hegemann, S.F. Kerstan, F. Lorenz, "Towards optimization under uncertainty for fundamental models in energy markets using quantum computers", arXiv:2301.01108
     
     Input:
     List of power unit parameters, precision, time steps, demand, costs, min up/down min/max supply parameters
     """
 
+    print("Start building UCP QUBO")
+
     qubostart = time.process_time()
 
 
     #calculating auxiliary variables
     dim=n*(pres+2)*T     #dimension of QUBO (size)
     dimt=n*(pres+2)      #size of one time step
 
@@ -1079,14 +1109,16 @@
     Build the relaxed QUBO for the unit commitment problem including uncertainty as outlined in the following paper:
     M.C. Braun, T. Decker, N. Hegemann, S.F. Kerstan, F. Lorenz, "Towards optimization under uncertainty for fundamental models in energy markets using quantum computers", arXiv:2301.01108
     
     Input:
     List of power unit parameters, precision, time steps, demand, costs, min up/down min/max supply parameters, list of demand and supply including probabilities from renewables
     """
 
+    print("Start building relaxed UCP QUBO")
+
     qubostart = time.process_time()
 
 
     #calculating auxiliary variables
     REres=len(pdRE[0][0])
     Dres=len(pdD[0])
     lREnum=len(pdRE[0])
@@ -1263,8 +1295,8 @@
             Qunique[dim+lRE+t*Dres+l][dim+lRE+t*Dres+l]=Qunique[dim+lRE+t*Dres+l][dim+lRE+t*Dres+l]-2*G
             for l2 in range(Dres):
                 Qunique[dim+lRE+t*Dres+l][dim+lRE+t*Dres+l2]=Qunique[dim+lRE+t*Dres+l][dim+lRE+t*Dres+l2]+G
 
     #if graphicsout==True:
     print('time to build QUBO:',time.process_time() - qubostart)                    #print Build time for QUBO
 
-    return   (Qcostq + Qstdemand + Qtmin + Qtdown + Qint1 + Qint2 + Qmdv + Qunique), Qcost
+    return   (Qcostq + Qstdemand + Qtmin + Qtdown + Qint1 + Qint2 + Qmdv + Qunique), Qcost
```

### Comparing `pygrnd-0.1.4/pygrnd/optimize/bruteforce.py` & `pygrnd-0.1.5/pygrnd/optimize/bruteforce.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/optimize/meritorder.py` & `pygrnd-0.1.5/pygrnd/optimize/meritorder.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/optimize/qaoa.py` & `pygrnd-0.1.5/pygrnd/optimize/qaoa.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/optimize/sat_ucp.py` & `pygrnd-0.1.5/pygrnd/optimize/sat_ucp.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/qc/MaximumLikelihoodForQAEwoPE.py` & `pygrnd-0.1.5/pygrnd/qc/MaximumLikelihoodForQAEwoPE.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/qc/QAE.py` & `pygrnd-0.1.5/pygrnd/qc/QAE.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/qc/brm.py` & `pygrnd-0.1.5/pygrnd/qc/brm.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/qc/brm_oracle.py` & `pygrnd-0.1.5/pygrnd/qc/brm_oracle.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/qc/brm_test.py` & `pygrnd-0.1.5/pygrnd/qc/brm_test.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/qc/circuitConstructor.py` & `pygrnd-0.1.5/pygrnd/qc/circuitConstructor.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/qc/circuitConstructor_test.py` & `pygrnd-0.1.5/pygrnd/qc/circuitConstructor_test.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/qc/helper.py` & `pygrnd-0.1.5/pygrnd/qc/helper.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/qc/lowDepthQAEgradientDescent.py` & `pygrnd-0.1.5/pygrnd/qc/lowDepthQAEgradientDescent.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,97 +27,96 @@
     angle2=2*math.pi-angle
     return min(angle1,angle2)
 
 #
 # Functions without the exponential error model.
 #
 
-def expectedProbability(theta, ell):
+def expectedProbabilityNoErrorModel(theta, ell):
     ''' Return the expected probability for a good state for angle theta
         and ell Grover operators after the initialization. No error model.
     '''
     return math.sin((2*ell+1)*theta/2)**2
 
-def errorAllPoints(theta, vectorN, vectorM, vectorR):
+def errorAllPointsNoErrorModel(theta, vectorN, vectorM, vectorR):
     ''' Return the sum of the squared deviations of the expected
         counts of good results and the measured results for the
         angle theta. vectorN contains the total counts, vectorM
         contains the number of Grover operators after the initialization
         and vectorR contains the counts of good states from the measurements.
         No error model.
     '''
     error=0.0
     for i in range(len(vectorN)):
         probMeasured=vectorR[i]/vectorN[i]
-        probExpected=expectedProbability(theta, vectorM[i])
+        probExpected=expectedProbabilityNoErrorModel(theta, vectorM[i])
         error=error+(probMeasured-probExpected)**2
     return error
 
-def gradientOptimizerVector(vectorN, vectorM, vectorR, thetaStart, stepSize):
+def gradientOptimizerVectorNoErrorModel(vectorN, vectorM, vectorR, thetaStart, stepSize, learningRate):
     ''' For given lists vectorN, vectorM and vectorR perform a gradient
-        descent search for the angle theta that minimizes errorAllPoints. The
-        method returns the angle and the corresponding error. Other
-        parameters are the step size and the start value for theta. No
-        error model.
+        descent search for the angle theta that minimizes errorAllPoints.
+        The method returns the angle and the corresponding error from the
+        deviation of the parameter fitting. Other parameters are the step
+        size for the gradient approximation, the learning rate and the start value for theta.
     '''
 
     # Initialize the search.
     bestTheta=thetaStart
-    bestError=errorAllPoints(thetaStart, vectorN, vectorM, vectorR)
+    bestError=errorAllPointsNoErrorModel(thetaStart, vectorN, vectorM, vectorR)
     continueFlag=True
 
     # Search as long we find an improvement.
     while continueFlag==True:
-        thetaPlus=bestTheta+stepSize
-        errorPlus=errorAllPoints(thetaPlus, vectorN, vectorM, vectorR)
+        bestThetaPrime=bestTheta+stepSize
+        error1=errorAllPointsNoErrorModel(bestThetaPrime, vectorN, vectorM, vectorR)
 
-        thetaMinus=bestTheta-stepSize
-        errorMinus=errorAllPoints(thetaMinus, vectorN, vectorM, vectorR)
+        gradientUnnormed=[(error1-bestError)/stepSize]
+        gradientNorm=sum(abs(x)**2 for x in gradientUnnormed)
+        gradientNormed=[x/math.sqrt(gradientNorm) for x in gradientUnnormed]
 
-        bestThetaLocal=thetaPlus
-        bestErrorLocal=errorPlus
+        thetaNew=bestTheta-learningRate*gradientNormed[0]
 
-        if errorMinus<bestErrorLocal:
-            bestThetaLocal=thetaMinus
-            bestErrorLocal=errorMinus
-
-        if bestErrorLocal<bestError:
-            bestTheta=bestThetaLocal
-            bestError=bestErrorLocal
+        errorNew=errorAllPointsNoErrorModel(thetaNew, vectorN, vectorM, vectorR)
+
+        if errorNew+0.000001<bestError:
+            bestError=errorNew
+            bestTheta=thetaNew
         else:
             continueFlag=False
+
     return bestTheta, bestError
 
-def loopGradientOptimizerVector(vectorN, vectorM, vectorR, rounds=10, stepSize=0.01):
+def loopGradientOptimizerVectorNoErrorModel(vectorN, vectorM, vectorR, rounds=10, stepSize=0.0001, learningRate=0.0001):
     ''' Run the gradient search for given vectorN, vectorM and vectorR. The search
         starts with random angles and has the specified number of rounds and step size.
         Returns the angle along with the corresponding probability estimation for the
         best result that was found.
     '''
 
     # Initialize search with random point.
-    theta=random.random()
-    bestTheta,bestError=gradientOptimizerVector(vectorN, vectorM, vectorR, theta, stepSize)
+    theta=2*math.pi*random.random()
+    bestTheta,bestError=gradientOptimizerVectorNoErrorModel(vectorN, vectorM, vectorR, theta, stepSize, learningRate)
 
     for i in range(rounds):
         theta=2*math.pi*random.random()
-        currentTheta,currentError=gradientOptimizerVector(vectorN, vectorM, vectorR, theta, stepSize)
+        currentTheta,currentError=gradientOptimizerVectorNoErrorModel(vectorN, vectorM, vectorR, theta, stepSize, learningRate)
         if currentError<bestError:
             bestTheta=currentTheta
             bestError=currentError
     return bestTheta, math.sin(bestTheta/2)**2
 
 #
 # Example for the gradient search of theta without error model.
 #
 # vectorN=[30, 30, 30, 30, 30, 30, 30, 30, 30]
 # vectorM=[ 0,  1,  2,  3,  4,  5,  6,  7,  8]
 # vectorR=[10, 29,  3, 21, 23,  0, 28, 10,  7]
 #
-# loopGradientOptimizerVector(vectorN, vectorM, vectorR, rounds=100, stepSize=0.0001)
+# loopGradientOptimizerVectorNoErrorModel(vectorN, vectorM, vectorR, rounds=100, stepSize=0.0001)
 
 
 #
 # Functions for the exponential error model.
 #
 
 def expectedProbabilityErrorModel(theta, ell, a, f):
@@ -143,15 +142,16 @@
     return error
 
 def gradientOptimizerVectorErrorModel(vectorN, vectorM, vectorR, thetaStart, aStart, fStart, stepSize, learningRate):
     ''' For given lists vectorN, vectorM and vectorR perform a gradient
         descent search for the angle theta and parameters a and f of the error model
         that minimizes errorAllPoints. The method returns the angle and the parameters of the
         error model and the corresponding error from the deviation of the parameter fitting.
-        Other parameters are the step size and the start value for theta.
+        Other parameters are the step size for the gradient approximation, the learning rate and
+        the start value for theta and the parameters of the error model.
     '''
 
     # Initialize the search.
     bestTheta=thetaStart
     bestA=aStart
     bestF=fStart
     bestError=errorAllPointsErrorModel(thetaStart, aStart, fStart, vectorN, vectorM, vectorR)
```

### Comparing `pygrnd-0.1.4/pygrnd/qc/optimize.py` & `pygrnd-0.1.5/pygrnd/qc/optimize.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/qc/parallelQAE.py` & `pygrnd-0.1.5/pygrnd/qc/parallelQAE.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/qc/patternGenerator.py` & `pygrnd-0.1.5/pygrnd/qc/patternGenerator.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/qc/patternReducer.py` & `pygrnd-0.1.5/pygrnd/qc/patternReducer.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.4/pygrnd/qc/probabilisticNetworks.py` & `pygrnd-0.1.5/pygrnd/qc/probabilisticNetworks.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 limitations under the License.'''
 
 import random
 import math
 import numpy as np
 from pygrnd.qc.helper import allCombinations, num2bin
 from qiskit import QuantumCircuit, QuantumRegister, ClassicalRegister, Aer, execute
-from qiskit.circuit.library import RYGate
+from qiskit.circuit.library import RYGate, ZGate
 
 def monteCarloEvaluation(timesteps, nodes, probFail, probRecovery, edges, rounds=100000):
     """ Evaluate a probabilistic network with a Monte Carlo simulation. The output
         is a list of probabilities for all possible configurations.
     """
     allRes={}
     for run in range(rounds):
@@ -288,7 +288,44 @@
     for c in allCombinations(len(nodes)):
         d=c[::-1]
         if d in res:
             res2.append(res[d])
         else:
             res2.append(0)
     return res2
+
+def constructGroverOperatorWithPhaseGateOnLastTimeStep(model, phaseGate, numberNodes):
+    ''' Construct the Grover operator for the model gate of a probabilistic network
+        model with time steps. The phase gate is applied to the part of the qubits
+        that correspond to the last time step. The number of nodes of the
+        network must be provided.
+    '''
+    numberQubits=model.num_qubits
+    qr=QuantumRegister(numberQubits,'q')
+    qc=QuantumCircuit(qr)
+
+    # mark the good states sequentially
+    qc.append(phaseGate,qr[-numberNodes:])
+
+    # Inverse operation
+    qc.append(model.inverse(),qr)
+
+    # Mark 0 with -1, include scalar -1 in front of formula
+    qc.x(qr[0])
+    qc.z(qr[0])
+    qc.x(qr[0])
+    qc.z(qr[0])
+    qc.x(qr[0])
+    if numberQubits>1:
+        qc.append(ZGate().control(num_ctrl_qubits=numberQubits-1,ctrl_state='0'*(numberQubits-1)),qr[1:]+[qr[0]])
+    else:
+        qc.z(qr[0])
+    qc.x(qr[0])
+
+    # Normal operation
+    qc.append(model,qr)
+
+    grover=qc.to_gate()
+    grover.label="Grover"
+
+    return grover
+
```

### Comparing `pygrnd-0.1.4/pygrnd/qc/qml.py` & `pygrnd-0.1.5/pygrnd/qc/qml.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
         through the whole training set (x_train, y_train). The training set is divided into
         training batches. Gradients are computed and weights updates at the end of each batch.
 
         Args:
             x_train (np.array):
                 Training inputs.
             y_train (np.array):
-                Training outputs. Must be elements of [0, 1].
+                Training outputs. Must be elements of [O, 1].
             x_test (np.array):
                 Testing inputs.
             y_test (np.array):
                 Testing outputs. Must be elements of [0, 1].
             epochs (int):
                 Number of training epochs.
             batch_size (int):
@@ -427,8 +427,8 @@
     def predict(self, x_list: np.array):
         """Returns the predictions (model outputs) for the given input data.
 
         Args:
             x_list (np.array):
                 Input data.
         """
-        return [self.qnode(self.weights, x) for x in x_list]
+        return [(self.qnode(self.weights, x)+ 1) / 2 for x in x_list]
```

### Comparing `pygrnd-0.1.4/pygrnd.egg-info/PKG-INFO` & `pygrnd-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,9 @@
-Metadata-Version: 2.1
-Name: pygrnd
-Version: 0.1.4
-Summary: A python library for quantum algorithms and software
-Home-page: https://github.com/JoSQUANTUM/pygrnd
-Author: JoS QUANTUM
-Author-email: contact@jos-quantum.de
-License: Apache 2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pygrnd 
-is a libary of various quantum algorithms written by the Team JoS QUANTUM GmbH to support the development of Applications for quantum computing in Finance, Insurance and Energy. The framework is a collection of open source libraries that enables building quantum models and prototypes and usage of our quantum algorithms.
+is a library of various quantum algorithms written by the Team JoS QUANTUM GmbH to support the development of Applications for quantum computing in Finance, Insurance and Energy. The framework is a collection of open source libraries that enables building quantum models and prototypes and usage of our quantum algorithms.
 
 pygrnd depends on different modules: 
 
     Quantum machine learning: pennylane (pennylane.ai/)
     Monte Carlo simulation: qiskit (qiskit.org)
     Optimization: qiskit, dimod (docs.ocean.dwavesys.com/en/stable/)
 
@@ -29,24 +15,27 @@
    
     pip install qiskit
     pip install numpy
     pip install dimod
     pip install dwave-greedy
     pip install pennylane
  
-# Tutorials
+# Tutorials and notebooks
+
+You can find example notebooks with usage of pygrnd functions in ``notebooks/``
 
 ## Quantum Risk Modelling
 
-Workflow to define a risk model like outlined in (https://arxiv.org/abs/2103.05475).
+Notebook: ``risk_model.ipynb`` and ``sensitivity_analysis.ipynb``
+
+Workflow to define a risk model like outlined in (<https://arxiv.org/abs/2103.05475>).
 Build a Grover operator with a state for which the overall probabilty should be evaluated.
 Standard Quantum Amplitude Estimation algorithm.
 Using QASM simulator you should not use more than 20 qubits (including the QAEqubits) on your local machine using simulator.
 
-
     - Input risk items, instrinsic and transition probabilities
     - List of states to estimate probabilities for the desired state
     - Precision for the QAE
     - Number of shots
 
 
 ### Syntax
@@ -108,14 +97,19 @@
 
     states, summe = modelProbabilities(nodes,edges,probsNodes,probsEdges)
     probsMonteCarlo = evaluateRiskModelMonteCarlo(nodes, edges, probsNodes, probsEdges, rounds)
 
 
 ## Amplitude Estimation without Phase Estimation
 
+Notebook: ``parallelQAE.ipynb``
+
+This notebook explaines functions for our proprietary quantum algorithm described in <https://arxiv.org/abs/2204.01337>.
+Parallel QAE is a quantum algorithm for Monte Carlo simulation on quantum computers with reduced gate depth and therefore a candidate to run quantum models on noisy quantum computers without full error-correction.
+
 - We have an operator A and a set of good results that have probability a in total.
 - We construct the Grover oracle G for A.
 - We construct a circuit with m calls of G in addition to one call of A and we run the circuit N times. We obtain h good results.
 - For different values of m we repeat this procedure.
 - We obtain vectors vectorN, vectorM and vectorH.
 - Use these parameters to guess the value a with maximum likelihood method.
 - The method uses a gradient descent with a random starting point and a stepSize=0.01 as default step size.
@@ -129,15 +123,19 @@
     vectorH = [21, 1, 29]
     bestTheta,bestProb = loopGradientOptimizerVector(vectorN, vectorM, vectorH, rounds=10, stepSize=0.01)
     print("best guess theta=",bestTheta)
     print("best guess prob=",bestProb)
 
 
 
-## Pattern-based Circuit optimizer
+## Pattern-based circuit optimizer
+
+Notebook: ``circuitConstructor.ipynb``
+
+The methods demonstrate how quantum circuits can be optimized to reduced gate depth. The methods are implementations or variations of algorithms of the following paper <https://doi.org/10.1103/PhysRevA.52.3457>. 
 
 ### Background: Patterns
 
 A pattern is an abstract representation of a sequence of quantum gates that corresponds to the identity. The gates are denoted by a string, e.g. H or X, and the parameters are variables or concrete values. The gates act on qubits that are denoted by numbers only.
 
 An example for a pattern:
 
@@ -204,29 +202,41 @@
 ## Quantum machine learing
 
 Quantum machine learning functions for regression and classifiction. 
 
 
 ### Example: Classification
 
-In ``notebooks/outlier_detection.ipynb`` an example for fraud detection (binary classification) based on a publicly available Kaggle data set is done.
+Notebook: ``notebooks/outlier_detection.ipynb`` 
+
+Example for fraud detection (binary classification) using parametrized quantum circuits to analyze a publicly available Kaggle data set.
 
 
 ### Example: Forecasting (coming soon)
 
 
 ### Example: Synthetic data (coming soon)
 
 
-
 ## Optimization
 
+
+
+Notebook ``ucp_relaxedQUBO.ipynb`` explaines the main idea of how to encode several variations of the Unit Commitment Problem (UCP, <https://en.wikipedia.org/wiki/Unit_commitment_problem_in_electrical_power_production>) as a QUBO (quadratic unconstrained binary optimization). 
+The UCP answers the following question: Which power generator should run at what level at which time to satisfy constrains like demand in each time step, power generator parameter like minimum and maximum up and down times and ramps. Because of growing amount of renewable energy grid in-feed, uncertainty of changing weather conditions requires fast precise solutions to the UCP. The notebook explains how the approach can be seen as a first attempt towards robust optimization by incorporating uncertainty from renewable energy supply. <https://arxiv.org/abs/2301.01108>
+
 Implementations of different QUBO (Quadratic Unconstrained Binary Optimization) solver for benchmarks.
 Methods for QUBO construction and solving. Classical brute-force solver, Monte Carlo, Quantum annealing (D-Wave), simulated annealing, Quantum approximate optimization algorithm.
 
+Notebook ``ucp_sat.ipynb`` explaines how to encode constraints as SAT formulation. THis construction is then mapped to a QUBO and several problem sets are benchmarked.
+
+Notebook ``merit_order.ipynb`` is the very first version of the merit order problem with power generator costs, static supply and demand formulated as knapsack.
+
+This work is based on the governmental funded project "EnerQuant":
+<https://ercim-news.ercim.eu/en128/special/energy-economics-fundamental-modelling-with-quantum-algorithms>
 
 ### Monte Carlo random search
 
 - randomly generate solution vector
 - calculation of matrix product x^T Q x
 - iterate N times
 
@@ -276,14 +286,16 @@
     Q = np.array([[10,-3,-4,-6],[-3,4,-2,-3],[-4,-2,6,-5],[-6,-3,-5,12]])
     N=10
     r,a=MCgradientSearch(Q,10)
     print(r,a)
 
 ### Quantum Approximate Optimization Algorithm (QAOA)
 
+A quantum algorithm to solve QUBO formulations on gate-based quantum computers. The function requires qiskit to construct circuits (qiskit high-level functions are not used).
+
 - input QUBO matrix as numpy array
 - build cost Hamiltonian U(gamma) using mapping x --> (x - 1) /2 (matrixConvertInv(m))
 - build mixer Hamiltonian U(beta)
 - construct one layer circuit with initial random beta, gamma values
 - execute on backend (default: Aer.get_backend('qasm_simulator'))
 - derive max count
 - calculate expectation value
```

### Comparing `pygrnd-0.1.4/pygrnd.egg-info/SOURCES.txt` & `pygrnd-0.1.5/pygrnd.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 pygrnd.egg-info/top_level.txt
 pygrnd/optimize/MonteCarloSolver.py
 pygrnd/optimize/UCPquboFunctionLibrary.py
 pygrnd/optimize/__init__.py
 pygrnd/optimize/bruteforce.py
 pygrnd/optimize/meritorder.py
 pygrnd/optimize/qaoa.py
+pygrnd/optimize/qmco.py
 pygrnd/optimize/sat_ucp.py
 pygrnd/qc/MaximumLikelihoodForQAEwoPE.py
 pygrnd/qc/QAE.py
 pygrnd/qc/__init__.py
 pygrnd/qc/brm.py
 pygrnd/qc/brm_oracle.py
 pygrnd/qc/brm_test.py
```

### Comparing `pygrnd-0.1.4/setup.py` & `pygrnd-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='pygrnd',
-    version='0.1.4',
+    version='0.1.5',
     description='A python library for quantum algorithms and software',
     long_description_content_type="text/markdown",
     long_description=long_description,
     url='https://github.com/JoSQUANTUM/pygrnd',
     author='JoS QUANTUM',
     author_email='contact@jos-quantum.de',
     license='Apache 2.0',
@@ -34,15 +34,20 @@
                       'numpy',
                       'dimod',
                       'dwave-greedy',
                       'pennylane>=0.27.0',
                       'pandas',
                       'seaborn',
                       'tqdm',
-                      'scikit-learn'
+                      'pylatexenc',
+                      'scikit-learn',
+                      'DateTime',
+                      'shap',
+                      'xgboost',
+                      'holidays'
                       ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent'
     ],
 )
```

