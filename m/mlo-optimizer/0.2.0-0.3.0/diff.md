# Comparing `tmp/mlo_optimizer-0.2.0.tar.gz` & `tmp/mlo_optimizer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlo_optimizer-0.2.0.tar", max compression
+gzip compressed data, was "mlo_optimizer-0.3.0.tar", max compression
```

## Comparing `mlo_optimizer-0.2.0.tar` & `mlo_optimizer-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11324 2023-04-04 09:09:40.411918 mlo_optimizer-0.2.0/LICENSE
--rw-r--r--   0        0        0       42 2023-04-04 08:56:55.904208 mlo_optimizer-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-09 13:50:59.589425 mlo_optimizer-0.2.0/mlo_optimizer/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 13:50:59.589425 mlo_optimizer-0.2.0/mlo_optimizer/components/__init__.py
--rwxr-xr-x   0        0        0     2081 2023-04-09 13:50:59.589425 mlo_optimizer-0.2.0/mlo_optimizer/components/algelitism.py
--rw-r--r--   0        0        0     3050 2023-04-09 13:50:59.593424 mlo_optimizer-0.2.0/mlo_optimizer/components/genetic_alg.py
--rw-r--r--   0        0        0      302 2023-04-09 16:34:08.728640 mlo_optimizer-0.2.0/mlo_optimizer/config.py
--rw-r--r--   0        0        0        0 2023-04-09 13:50:59.593424 mlo_optimizer-0.2.0/mlo_optimizer/data/__init__.py
--rw-r--r--   0        0        0      481 2023-04-09 13:50:59.593424 mlo_optimizer-0.2.0/mlo_optimizer/data/read.py
--rw-r--r--   0        0        0        0 2023-04-09 13:50:59.593424 mlo_optimizer-0.2.0/mlo_optimizer/keyboards/__init__.py
--rw-r--r--   0        0        0     2300 2023-04-09 13:50:59.593424 mlo_optimizer-0.2.0/mlo_optimizer/keyboards/bigrams.py
--rw-r--r--   0        0        0     2047 2023-04-09 16:45:19.841150 mlo_optimizer-0.2.0/mlo_optimizer/keyboards/distances.py
--rw-r--r--   0        0        0      663 2023-04-09 13:50:59.593424 mlo_optimizer-0.2.0/mlo_optimizer/keyboards/fitness.py
--rw-r--r--   0        0        0     9461 2023-04-09 16:45:19.841150 mlo_optimizer-0.2.0/mlo_optimizer/optimizer.py
--rw-r--r--   0        0        0      968 2023-04-09 16:47:20.995942 mlo_optimizer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 mlo_optimizer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11324 2023-04-04 09:09:40.411918 mlo_optimizer-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6836 2023-04-18 16:05:42.796312 mlo_optimizer-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 13:50:59.589425 mlo_optimizer-0.3.0/mlo_optimizer/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 13:50:59.589425 mlo_optimizer-0.3.0/mlo_optimizer/components/__init__.py
+-rwxr-xr-x   0        0        0     2081 2023-04-09 13:50:59.589425 mlo_optimizer-0.3.0/mlo_optimizer/components/algelitism.py
+-rw-r--r--   0        0        0     4129 2023-04-18 16:05:42.796312 mlo_optimizer-0.3.0/mlo_optimizer/components/genetic_alg.py
+-rw-r--r--   0        0        0      304 2023-04-18 16:05:42.796312 mlo_optimizer-0.3.0/mlo_optimizer/config.py
+-rw-r--r--   0        0        0        0 2023-04-09 13:50:59.593424 mlo_optimizer-0.3.0/mlo_optimizer/data/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-18 16:05:42.796312 mlo_optimizer-0.3.0/mlo_optimizer/data/read.py
+-rw-r--r--   0        0        0        0 2023-04-09 13:50:59.593424 mlo_optimizer-0.3.0/mlo_optimizer/keyboards/__init__.py
+-rw-r--r--   0        0        0     3681 2023-04-18 16:05:42.796312 mlo_optimizer-0.3.0/mlo_optimizer/keyboards/bigrams.py
+-rw-r--r--   0        0        0     3977 2023-04-18 16:05:42.796312 mlo_optimizer-0.3.0/mlo_optimizer/keyboards/distances.py
+-rw-r--r--   0        0        0     1899 2023-04-18 16:05:42.796312 mlo_optimizer-0.3.0/mlo_optimizer/keyboards/fitness.py
+-rw-r--r--   0        0        0    11376 2023-04-18 16:05:42.796312 mlo_optimizer-0.3.0/mlo_optimizer/optimizer.py
+-rw-r--r--   0        0        0      967 2023-04-18 16:09:07.059759 mlo_optimizer-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7547 1970-01-01 00:00:00.000000 mlo_optimizer-0.3.0/PKG-INFO
```

### Comparing `mlo_optimizer-0.2.0/LICENSE` & `mlo_optimizer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlo_optimizer-0.2.0/mlo_optimizer/components/algelitism.py` & `mlo_optimizer-0.3.0/mlo_optimizer/components/algelitism.py`

 * *Files identical despite different names*

### Comparing `mlo_optimizer-0.2.0/mlo_optimizer/keyboards/bigrams.py` & `mlo_optimizer-0.3.0/mlo_optimizer/keyboards/bigrams.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,28 +8,40 @@
 
 import pandas as pd
 
 from tqdm import tqdm
 
 
 def tokenize_by_letters(texts: pd.Series) -> list:
+    """Separates texts by character
+
+    :param texts: Series with strings from text files
+    :type texts: class:`pandas.Series`
+    :return: List of all characters
+    """
     tokenized_text = []
 
     print('Tokenization...')
     for i in tqdm(range(0, len(texts), BATCH_SIZE)):
         texts_batch = texts[i:i + BATCH_SIZE]
 
         for sentence in texts_batch:
             for letter in str(sentence).lower():
                 tokenized_text.append(letter)
 
     return tokenized_text
 
 
 def get_bigram_probs(tokenized_text: list) -> list:
+    """Calculates the probabilities of bigrams from each combination of two keys
+
+    :param tokenized_text: List of all texts separated by characters
+    :type tokenized_text: list
+    :return: List of bigrams of the form: ((first symbol, next symbol), probability)
+    """
     print('Getting bigrams...')
     bigrams = nltk.bigrams(tokenized_text)
     print('Calculation of bigram frequencies...')
     freq_dists = nltk.FreqDist(bigrams)
     print('Calculation of bigram probabilities...')
     prob_dists = nltk.MLEProbDist(freq_dists)
 
@@ -37,40 +49,62 @@
     print('Combining bigrams and their frequencies')
     for sample in tqdm(freq_dists.keys()):
         bigram_probs.append((sample, prob_dists.prob(sample)))
 
     return bigram_probs
 
 
-def filter_bigram_probs(bigram_probs: list, counted_keys: list) -> list:
+def filter_bigram_probs(bigram_probs: list, counted_elems: list) -> list:
+    """Removes bigrams that are not in the counted_keys
+
+    :param bigram_probs: List of bigrams of the form: ((first symbol, next symbol), probability)
+    :type bigram_probs list
+    :param counted_elems: Set of elements taken into account in the objective function
+    :type counted_elems: list
+    :return: List of filtered bigrams
+    """
     filtered_bigram_probs = []
 
     print('Bigram filtering...')
     for bigram in tqdm(bigram_probs):
         new_bigram = [bigram[0][0], bigram[0][1]]
 
         if bigram[0][0] == ' ':
             new_bigram[0] = 'space'
         if bigram[0][1] == ' ':
             new_bigram[1] = 'space'
         if bigram[0][0] == '\n':
             new_bigram[0] = 'enter'
         if bigram[0][1] == '\n':
             new_bigram[1] = 'enter'
-        if new_bigram[0] in counted_keys and new_bigram[1] in counted_keys:
+        if new_bigram[0] in counted_elems and new_bigram[1] in counted_elems:
             filtered_bigram_probs.append(((new_bigram[0], new_bigram[1]), bigram[1]))
 
     return filtered_bigram_probs
 
 
 def get_bigram_probs_vec(bigram_probs: list) -> np.array:
+    """Separates the vector of bigrams from the list of bigrams
+
+    :param bigram_probs: List of bigrams of the form: ((first symbol, next symbol), probability)
+    :type bigram_probs: list
+    :return: Bigram vector
+    """
     if bigram_probs is not None:
         return np.array([elem[1] for elem in bigram_probs])
 
 
 def get_bigram_probs_with_vec(texts: pd.Series, counted_elems: list) -> Tuple[list, np.array]:
+    """Launches a full pipeline with the calculation of lists of probabilities of bigrams
+
+    :param texts: Separates texts by character
+    :type texts: class:`pandas.Series`
+    :param counted_elems: Set of elements taken into account in the objective function
+    :type counted_elems: list
+    :return: List of filtered bigrams and bigram vector
+    """
     tokenized_text = tokenize_by_letters(texts)
     bigram_probs = get_bigram_probs(tokenized_text)
     filtered_bigram_probs = filter_bigram_probs(bigram_probs, counted_elems)
     filtered_bigram_probs_vec = get_bigram_probs_vec(filtered_bigram_probs)
 
     return filtered_bigram_probs, filtered_bigram_probs_vec
```

### Comparing `mlo_optimizer-0.2.0/mlo_optimizer/optimizer.py` & `mlo_optimizer-0.3.0/mlo_optimizer/optimizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -93,18 +93,47 @@
         self.name = '__x'
 
     def __get__(self, instance, owner):
         return getattr(instance, self.name)
 
 
 class Optimizer:
-    """Тестовая документация
+    """Main class that tunes the components of the genetic algorithm and implements the optimizer
 
-    :param init_matrix: Класс состояний, хранящий изменяемые флаги и выбранные раскладки
+    :param init_matrix: Initial initialization matrix with elements (permutable and not counted)
     :type init_matrix: list
+    :param counted_elems: Set of elements taken into account in the objective function
+    :type counted_elems: list
+    :param permutable_elems: The set of elements that are rearranged during crossover and mutation
+    :type permutable_elems: list
+    :param fitness_func: Objective function that receives an individual as input and returns a fitness score
+    :type fitness_func: callable
+    :param fitness_func_kwargs: Named arguments for target function
+    :type fitness_func_kwargs: dict
+    :param minimization: Minimization and Maximization Flag of the Objective Function
+    :type minimization: bool
+    :param a_s: Half side of square button (when fitness_func='square')
+    :type a_s: float
+    :param a_h: Distance from the middle of a hexagonal key to the middle of its side (when fitness_func='hex')
+    :type a_h: float
+    :param b_h: Distance from the middle of the hexagonal key to the middle of the side of the bottom key (when
+    fitness_func='hex')
+    :type b_h: float
+    :param population_size: Population size in one generation
+    :type population_size: int
+    :param p_crossover: Crossbreeding probability
+    :type p_crossover: float
+    :param p_mutation: Mutation probability
+    :type p_mutation: float
+    :param max_generation: Maximum number of generations
+    :type max_generation: int
+    :param tourn_size: sample size for tournament selection
+    :type tourn_size: int
+    :param hall_of_fame_size: Number of best individuals obtained after the completion of the optimization
+    :type hall_of_fame_size: int
     """
     IMPLEMENTED_FITNESS_FUNCS = ('square', 'hex')
 
     init_matrix = ListDescriptor()
     counted_elems = ListDescriptor()
     permutable_elems = ListDescriptor()
     a_s = CoefficientDescriptor()
@@ -120,51 +149,60 @@
     bigram_probs = BigramProbsDescriptor()
     get_bigram_probs_with_vec = BigramProbsDescriptor()
 
     def __init__(self,
                  init_matrix: list,
                  counted_elems: list,
                  permutable_elems: list,
-                 fitness_func=FITNESS_FUNC_DEFAULT,
+                 fitness_func: callable = FITNESS_FUNC_DEFAULT,
                  fitness_func_kwargs: dict = None,
                  minimization: bool = MINIMIZATION_DEFAULT,
                  a_s: float = A_S_DEFAULT,
                  a_h: float = A_H_DEFAULT,
                  b_h: float = B_H_DEFAULT,
                  population_size: int = POPULATION_SIZE_DEFAULT,
+                 max_generation: int = MAX_GENERATION_DEFAULT,
                  p_crossover: float = P_CROSSOVER_DEFAULT,
                  p_mutation: float = P_MUTATION_DEFAULT,
-                 max_generation: int = MAX_GENERATION_DEFAULT,
                  tourn_size: int = TOURN_SIZE_DEFAULT,
                  hall_of_fame_size: int = HALL_OF_FAME_SIZE_DEFAULT):
 
         self.init_matrix = init_matrix
         self.counted_elems = counted_elems
         self.permutable_elems = permutable_elems
         self.fitness_func = fitness_func
         self.fitness_func_kwargs = fitness_func_kwargs
         self.minimization = minimization
         self.a_s = a_s
         self.a_h = a_h
         self.b_h = b_h
         self.population_size = population_size
         self.max_generation = max_generation
-        self.tourn_size = tourn_size
-        self.hall_of_fame_size = hall_of_fame_size
         self.p_crossover = p_crossover
         self.p_mutation = p_mutation
+        self.tourn_size = tourn_size
+        self.hall_of_fame_size = hall_of_fame_size
 
         self.bigram_probs = None
         self.bigram_probs_vec = None
 
     def fit_bigrams(self, lang_part_dir: str):
+        """Reads text files and construct bigram probability vectors from them
+
+        :param lang_part_dir: Folder with text files
+        :type lang_part_dir: str
+        """
         texts = read_dir(lang_part_dir)
         self.bigram_probs, self.bigram_probs_vec = get_bigram_probs_with_vec(texts, self.counted_elems)
 
     def optimize(self):
+        """Collects all components and runs optimization
+
+        :return: Matrices of the best individuals (quantity depends on the parameter hall_of_fame_size)
+        """
         if self.__minimization:
             weight = -1.0
         else:
             weight = 1.0
 
         creator.create('FitnessMin', base.Fitness, weights=(weight,))
         creator.create('Individual', list, fitness=creator.FitnessMin)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mlo_optimizer-0.2.0/pyproject.toml` & `mlo_optimizer-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "mlo-optimizer"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Jaskier <borody.maxim@gmail.com>"]
 keywords = ["matrix", "optimization", "genetic", "keyboard"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [
     {include = "mlo_optimizer"}
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.11,<3.12"
+python = ">=3.9,<3.12"
 numpy = "^1.24.2"
 pandas = "^2.0.0"
 tqdm = "^4.65.0"
 nltk = "^3.8.1"
 deap = "^1.3.3"
```

