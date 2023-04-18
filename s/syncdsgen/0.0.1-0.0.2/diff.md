# Comparing `tmp/syncdsgen-0.0.1.tar.gz` & `tmp/syncdsgen-0.0.2.tar.gz`

## Comparing `syncdsgen-0.0.1.tar` & `syncdsgen-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rwxr-xr-x   0        0        0    10936 2020-02-02 00:00:00.000000 syncdsgen-0.0.1/syncdsgen_demo.ipynb
--rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 syncdsgen-0.0.1/.vscode/settings.json
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 syncdsgen-0.0.1/SynCDsGen/__init__.py
--rwxr-xr-x   0        0        0     9732 2020-02-02 00:00:00.000000 syncdsgen-0.0.1/SynCDsGen/syncdsgen.py
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 syncdsgen-0.0.1/.gitignore
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 syncdsgen-0.0.1/LICENCE
--rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 syncdsgen-0.0.1/README.md
--rwxr-xr-x   0        0        0      532 2020-02-02 00:00:00.000000 syncdsgen-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 syncdsgen-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     2063 2020-02-02 00:00:00.000000 syncdsgen-0.0.2/requirements.txt
+-rwxr-xr-x   0        0        0     9221 2020-02-02 00:00:00.000000 syncdsgen-0.0.2/syncdsgen_demo.ipynb
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 syncdsgen-0.0.2/.vscode/settings.json
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 syncdsgen-0.0.2/SynCDsGen/__init__.py
+-rwxr-xr-x   0        0        0    13147 2020-02-02 00:00:00.000000 syncdsgen-0.0.2/SynCDsGen/syncdsgen.py
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 syncdsgen-0.0.2/.gitignore
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 syncdsgen-0.0.2/LICENCE
+-rwxr-xr-x   0        0        0      479 2020-02-02 00:00:00.000000 syncdsgen-0.0.2/README.md
+-rwxr-xr-x   0        0        0      532 2020-02-02 00:00:00.000000 syncdsgen-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 syncdsgen-0.0.2/PKG-INFO
```

### Comparing `syncdsgen-0.0.1/syncdsgen_demo.ipynb` & `syncdsgen-0.0.2/syncdsgen_demo.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9854855121824897%*

 * *Differences: {"'cells'": "{2: {'execution_count': 4, 'outputs': []}, 5: {'source': {insert: [(3, "*

 * *            '"conf.codons = [\'aa\', \'ab\', \'ac\', \'ba\', \'ca\', \'bb\', \'bc\', \'cb\']\\n"), '*

 * *            '(5, "conf.stop_codons = [\'ac\']\\n"), (13, \'conf.transition_prob_t = '*

 * *            "torch.Tensor([[0,  0, 1/2, 1/2],\\n'), (14, '                            [0, 0, 1/2, "*

 * *            "1/2],\\n'), (15, '                            [0, 0, 1/2, 1/2],\\n'), (16, "*

 * *            "'                            [0, 0,  […]*

```diff
@@ -14,26 +14,17 @@
             "metadata": {},
             "source": [
                 "The goal of this notebook is to show how to use the SynCDsGen module."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 4,
             "metadata": {},
-            "outputs": [
-                {
-                    "ename": "",
-                    "evalue": "",
-                    "output_type": "error",
-                    "traceback": [
-                        "\u001b[1;31mLe Kernel s\u2019est bloqu\u00e9 lors de l\u2019ex\u00e9cution du code dans la cellule active ou une cellule pr\u00e9c\u00e9dente. Veuillez v\u00e9rifier le code dans la ou les cellules pour identifier une cause possible de l\u2019\u00e9chec. Cliquez <a href='https://aka.ms/vscodeJupyterKernelCrash'>ici</a> pour plus d\u2019informations. Pour plus d\u2019informations, consultez Jupyter <a href='command:jupyter.viewOutput'>log</a>."
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "exit()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
@@ -58,49 +49,49 @@
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "conf = SynCDsGen.SyncCDsGeneratorConf()\n",
                 "\n",
                 "conf.bases = ['a', 'b', 'c']\n",
-                "conf.codons = ['aa', 'ab', 'ac', 'ba', 'ca', 'bb', 'bc', 'cb', 'cc']\n",
+                "conf.codons = ['aa', 'ab', 'ac', 'ba', 'ca', 'bb', 'bc', 'cb']\n",
                 "conf.start_codons = ['aa', 'ab']\n",
-                "#STOP_CODONS = ['cc']\n",
+                "conf.stop_codons = ['ac']\n",
                 "conf.AAs = ['A', 'B', 'C', 'D']\n",
                 "conf.translation_dict = {\n",
                 "    'A':  ['aa', 'ab'],\n",
                 "    'B': ['ac'],\n",
                 "    'C': ['ba', 'bc', 'cb'],\n",
                 "    'D': ['ca', 'bb']\n",
                 "}\n",
-                "conf.transition_prob_t = torch.Tensor([[0,  1/3, 1/3, 1/3],\n",
-                "                            [0, 1/3, 1/3, 1/3],\n",
-                "                            [0, 1/3, 1/3, 1/3],\n",
-                "                            [0, 1/3, 1/3, 1/3]])\n",
+                "conf.transition_prob_t = torch.Tensor([[0,  0, 1/2, 1/2],\n",
+                "                            [0, 0, 1/2, 1/2],\n",
+                "                            [0, 0, 1/2, 1/2],\n",
+                "                            [0, 0, 1/2, 1/2]])\n",
                 "\n",
                 "conf.emission_prob_t = torch.Tensor([[1/2, 1/2, 0.0],\n",
                 "                          [1, 0.0, 0.0],\n",
                 "                          [0.6, 0.2, 0.2],\n",
                 "                          [0.7, 0.3, 0.0]])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
                 "generator = SynCDsGen.StochasticSynCDsGenerator(conf)\n",
                 "\n",
-                "synthetic_data = generator.sample()"
+                "synthetic_data = generator.sample(length=5)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -123,58 +114,51 @@
                             "      <th>AAs</th>\n",
                             "      <th>CDs</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>ACCBCBDDCBBDCDDDCCBBCDBCDCCBDBCCBBCCDCBBDCCCBDCDC</td>\n",
-                            "      <td>abbacbacbcaccacacbacaccabacacabbbcbaacacbabbac...</td>\n",
+                            "      <td>ADCB</td>\n",
+                            "      <td>aacabaac</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>ACDDBBCCCBCDDBBCBDBCBCDBCDBDDCBCBDBBDBBDDBBDCBBDD</td>\n",
-                            "      <td>abbabbcaacacbabccbacbacacaacacbcaccaacbaaccbbb...</td>\n",
+                            "      <td>ADCB</td>\n",
+                            "      <td>aacabcac</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>ABCBCDBBCDCDCBDCBCBBCDBBCBDBCCCCDDBCDCCBDBDCCCCBC</td>\n",
-                            "      <td>abacbcaccbcaacacbccacbcabcaccabcacbaacacbcbbac...</td>\n",
+                            "      <td>ACDB</td>\n",
+                            "      <td>abcbcaac</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>ABCBDBBCCDBDDDCCDDCDBDBCCBCBCCDCBDCCDBCCDCDBCDBDB</td>\n",
-                            "      <td>aaacbaaccaacacbccbcaaccacacababccacabacaaccaac...</td>\n",
+                            "      <td>ADCB</td>\n",
+                            "      <td>aabbbaac</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>ABCCBDBBCCDCBDBBBDBBDBBDDDBBDDBBDDDBDCDDBBBCBBDDB</td>\n",
-                            "      <td>abacbabaacbbacacbcbacabcaccaacacacbbacacbbacac...</td>\n",
+                            "      <td>ADCB</td>\n",
+                            "      <td>abcabcac</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "                                                 AAs  \\\n",
-                            "0  ACCBCBDDCBBDCDDDCCBBCDBCDCCBDBCCBBCCDCBBDCCCBDCDC   \n",
-                            "1  ACDDBBCCCBCDDBBCBDBCBCDBCDBDDCBCBDBBDBBDDBBDCBBDD   \n",
-                            "2  ABCBCDBBCDCDCBDCBCBBCDBBCBDBCCCCDDBCDCCBDBDCCCCBC   \n",
-                            "3  ABCBDBBCCDBDDDCCDDCDBDBCCBCBCCDCBDCCDBCCDCDBCDBDB   \n",
-                            "4  ABCCBDBBCCDCBDBBBDBBDBBDDDBBDDBBDDDBDCDDBBBCBBDDB   \n",
-                            "\n",
-                            "                                                 CDs  \n",
-                            "0  abbacbacbcaccacacbacaccabacacabbbcbaacacbabbac...  \n",
-                            "1  abbabbcaacacbabccbacbacacaacacbcaccaacbaaccbbb...  \n",
-                            "2  abacbcaccbcaacacbccacbcabcaccabcacbaacacbcbbac...  \n",
-                            "3  aaacbaaccaacacbccbcaaccacacababccacabacaaccaac...  \n",
-                            "4  abacbabaacbbacacbcbacabcaccaacacacbbacacbbacac...  "
+                            "    AAs       CDs\n",
+                            "0  ADCB  aacabaac\n",
+                            "1  ADCB  aacabcac\n",
+                            "2  ACDB  abcbcaac\n",
+                            "3  ADCB  aabbbaac\n",
+                            "4  ADCB  abcabcac"
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "synthetic_data.head()"
             ]
@@ -317,21 +301,14 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "synthetic_data.head()"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "venv",
             "language": "python",
             "name": "python3"
```

### Comparing `syncdsgen-0.0.1/SynCDsGen/syncdsgen.py` & `syncdsgen-0.0.2/SynCDsGen/syncdsgen.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,111 @@
+#import useful modules
 import torch
 import pyro
 import pandas as pd
 import numpy as np
 import re
+from enum import Enum
 
 def check_row_sum(tensor, tol=1e-6):
-        row_sums = tensor.sum(dim=1)
-        return torch.all(torch.abs(row_sums - 1) < tol)
+    """
+        Function to check if each row of a given tensor sum up to 1
+    """
+    row_sums = tensor.sum(dim=1)
+    return torch.all(torch.abs(row_sums - 1) < tol)
+
 
 class SyncCDsGeneratorConf:
     def __init__(self, bases=None, codons=None, start_codons=None,
                   stop_codons=None, AAs=None, translation_dict=None,
                   transition_prob_t=None, emission_prob_t=None, AAs_initial_prob_dist=None,
-                  codon_length=None, constraints_dict=None):
+                  codon_length=None, constraints_dict=None, AAs_stop_prob_dist=None):
+        """
+        Initialize a new instance of SyncCDsGeneratorConf
+
+        Args:
+            bases (list): list of bases
+            codons (list): list of codons
+            start_codons (list): list of start codons
+            stop_codons (list): list of stop codons
+        """
         self.bases = bases
         self.codons = codons
         self.start_codons = start_codons
         self.stop_codons = stop_codons
         self.AAs = AAs
         self.translation_dict = translation_dict
         self.transition_prob_t = transition_prob_t
         self.emission_prob_t = emission_prob_t
         self.AAs_initial_prob_dist = AAs_initial_prob_dist
         self.codon_length = codon_length
         self.constraints_dict = constraints_dict
+        self.AAs_stop_prob_dist = AAs_stop_prob_dist
 
     def is_AA_start_AA(self, AA):
         coding_codons = self.translation_dict[AA]
 
         for codon in coding_codons:
             if codon in self.start_codons:
                 return 1
         return 0
+    
+    def is_AA_stop_AA(self, AA):
+        """
+            Function to check if a given amino acid is encoded by a stop codon
+
+            Returns True if AA is encoded by stop codons and False otherwise
+        """
+        coding_codons = self.translation_dict[AA]
+
+        for codon in coding_codons:
+            if codon in self.stop_codons:
+                return 1
+        return 0
 
     def get_AAs_initial_prob_dist(self):
         start_codons_prob_dist = [self.is_AA_start_AA(AA) for AA in self.AAs]
         nb_start_AAs = start_codons_prob_dist.count(1)
 
         start_codons_prob_dist = np.array(start_codons_prob_dist)/ nb_start_AAs
 
         return(start_codons_prob_dist)
+    
+    def get_AAs_stop_prob_dist(self):
+        """
+            Function to compute the distribution probability of stop AAs
+
+            Returns a numpy array of the size of the array AAs. The arrays indicates the probability
+            of appearance of each AA as a stop codon at the end of a sequence; AAs encoded by stop
+            codons have the same probability of appearance, and the others have a 0 probability of
+            appearance
+        """
+        stop_codons_prob_dist = [self.is_AA_stop_AA(AA) for AA in self.AAs]
+        nb_stop_AAs = stop_codons_prob_dist.count(1)
+
+        stop_codons_prob_dist = np.array(stop_codons_prob_dist)/ nb_stop_AAs
 
+        return(stop_codons_prob_dist)
+
+class Position(Enum):
+        START = 1
+        STOP = 2
 
 class SynCDsGenerator:
     def __init__(self, generatorConf:SyncCDsGeneratorConf):
         self.generatorConf = generatorConf
         self.AAs_indices_sequences = []
         self.CDs_indices_sequences = []
 
         #check the validity of the attributes of the generator configuration
-        assert len(generatorConf.start_codons) > 0, "For yncCDsGeneratorConf, the list of start codons should not be empty" #the list of start codons should not be emtpy
+        assert all(c in self.generatorConf.bases for codon in self.generatorConf.codons for c in codon), "The characters used for codons should be in the list of SyncCDsGeneratorConf.bases"
+        assert len(generatorConf.start_codons) > 0, "For yncCDsGeneratorConf, the list of start codons should not be empty"
+        assert all(codon in self.generatorConf.codons for codon in self.generatorConf.start_codons), "Start codons should be a subset of codons"
+        assert all(codon in self.generatorConf.codons for codon in self.generatorConf.stop_codons), "Stop codons should be a subset of codons"
+        assert len(generatorConf.stop_codons) > 0, "For yncCDsGeneratorConf, the list of stop codons should not be empty"
         assert len(generatorConf.translation_dict) == len(generatorConf.AAs), "For yncCDsGeneratorConf, translation dict should have the same size with the AAs list" #the translation_dict and the AAs list should have the same size
         assert generatorConf.transition_prob_t.size()[0] == generatorConf.transition_prob_t.size()[1] == len(generatorConf.AAs), "The emission_prob_t should be a squared tensor, and its size should be equal to the size of the AAs list"
 
         max_nb_syn_codons = max([len(syn_codons) for syn_codons in self.generatorConf.translation_dict.values()])
         assert generatorConf.emission_prob_t.size()[1] == max_nb_syn_codons, f"The second dimension of the emission_prob_t tensor should be {max_nb_syn_codons}, got {generatorConf.emission_prob_t.size()[1]}"
         
         assert check_row_sum(self.generatorConf.emission_prob_t), "Each row of the emission_prob_t should sum up to 1"
@@ -62,76 +114,105 @@
         if self.generatorConf.codon_length is None:
             l = len(self.generatorConf.codons[0])
             assert all(len(codon) == l for codon in self.generatorConf.codons), f"All the codons should have the same length"
             self.generatorConf.codon_length = l
         else:
             assert all(len(codon) == self.generatorConf.codon_length for codon in self.generatorConf.codons), f"All the codons should have the same length, since the codon length had been set to {self.generatorConf.codon_length}"
 
+        if self.generatorConf.AAs_initial_prob_dist is None:
+            self.generatorConf.AAs_initial_prob_dist = self.generatorConf.get_AAs_initial_prob_dist()
+        else:
+            assert np.sum(self.generatorConf.AAs_initial_prob_dist)==1, f"AAs_stop_prob_dist should sum up to 1, got {np.sum(self.generatorConf.AAs_stop_prob_dist)}"
+
+        if self.generatorConf.AAs_stop_prob_dist is None:
+            self.generatorConf.AAs_stop_prob_dist = self.generatorConf.get_AAs_stop_prob_dist()
+        else:
+            assert np.sum(self.generatorConf.AAs_stop_prob_dist)==1, f"AAs_stop_prob_dist should sum up to 1, got {np.sum(self.generatorConf.AAs_stop_prob_dist)}"
+    
     def AA_indices_sequence_to_AA_sequence(self, X):
         return ''.join([self.generatorConf.AAs[i] for i in X])
 
     def CD_indices_sequence_to_CD_sequence(self, X):
         """
             input:
                 X: list of indices of the AAs of the sequence concate to the list of indices of the codons of the sequence
         """
         N = len(X)
         AA_ind,  CDs_ind = X[0:N//2], X[N//2:]
 
         return ''.join([self.generatorConf.translation_dict[self.generatorConf.AAs[a]][int(i)] for a, i in zip(AA_ind, CDs_ind)])
     
+    def generate_token(self, position:Position):
+        """
+            Function to generate the start token of a sequence
+
+            Returns the start AA and the corresponding codon
+        """
+        assert position in (Position.START, Position.STOP), "position should be an instance of the Position class"
+        
+        if position == Position.START:
+            prob_t = self.generatorConf.AAs_initial_prob_dist
+            names = ["x_start", "y_start"]
+        elif position == Position.STOP:
+            prob_t = self.generatorConf.AAs_stop_prob_dist
+            names = ["x_end", "y_end"]
+
+        state = pyro.sample(names[0],
+                                pyro.distributions.Categorical(torch.Tensor(prob_t)))
+        emission_p_t = self.generatorConf.emission_prob_t[state]
+
+        observation = pyro.sample(names[1],
+                                    pyro.distributions.Categorical(emission_p_t))
+
+        return state, observation
+    
     def build_dataframe(self):
         AAs_sequences = np.apply_along_axis(self.AA_indices_sequence_to_AA_sequence, 1, self.AAs_indices_sequences)
 
         joined_sequences = np.hstack((self.AAs_indices_sequences, self.CDs__indices_sequences))
         CDs_sequences = np.apply_along_axis(self.CD_indices_sequence_to_CD_sequence, 1, joined_sequences)
 
         self.synthetic_data = pd.DataFrame({'AAs': AAs_sequences, 'CDs': CDs_sequences})
 
 
 class StochasticSynCDsGenerator(SynCDsGenerator):
     def __init__(self, generatorConf:SyncCDsGeneratorConf):
-        super().init__(generatorConf)
+        super().__init__(generatorConf)
 
     def sample(self, n_samples=100, length=50):
-
-        if self.generatorConf.AAs_initial_prob_dist is None:
-            self.generatorConf.AAs_initial_prob_dist = self.generatorConf.get_AAs_initial_prob_dist()
-
         assert length > 3, f"Waiting length > 3, got {length}"
 
         AAs_samples = []
         CDs_samples = []
 
         for j in torch.arange(0, n_samples):
             hidden_states = []
             observations = []
 
             #generate the first AA of the AA sequence from the start codons
-            state = pyro.sample("x_{}_0".format(j),
-                                pyro.distributions.Categorical(torch.Tensor(self.generatorConf.AAs_initial_prob_dist)))
-            emission_p_t = self.generatorConf.emission_prob_t[state]
-
-            observation = pyro.sample("y_{}_0".format(j),
-                                      pyro.distributions.Categorical(emission_p_t))
-            
+            state, observation = self.generate_token(Position.START)
             hidden_states.append(state)
             observations.append(observation)
 
-            for k in torch.arange(1, length-1):
+            for k in torch.arange(1, length-2):
                 transition_p_t = self.generatorConf.transition_prob_t[state]
                 state = pyro.sample("x_{}_{}".format(j, k),
                                     pyro.distributions.Categorical(transition_p_t))
                 emission_p_t = self.generatorConf.emission_prob_t[state]
 
                 observation = pyro.sample("y_{}_{}".format(j, k),
                                           pyro.distributions.Categorical(emission_p_t))
 
                 hidden_states.append(state)
                 observations.append(observation)   
+            
+            #generate the stop codon
+            state, observation = self.generate_token(Position.STOP)
+            hidden_states.append(state)
+            observations.append(observation)   
 
             AA_sample = torch.Tensor(hidden_states)
             CDs_sample = torch.Tensor(observations)
 
             AAs_samples.append(AA_sample)
             CDs_samples.append(CDs_sample)
 
@@ -162,25 +243,19 @@
         CDs_samples = []
 
         for j in torch.arange(0, n_samples):
             hidden_states = []
             observations = []
 
             #generate the first AA of the AA sequence from the start codons
-            state = pyro.sample("x_{}_0".format(j),
-                                pyro.distributions.Categorical(torch.Tensor(self.generatorConf.AAs_initial_prob_dist)))
-            emission_p_t = self.generatorConf.emission_prob_t[state]
-
-            observation = pyro.sample("y_{}_0".format(j),
-                                      pyro.distributions.Categorical(emission_p_t))
-            
+            state, observation = self.generate_token(Position.START)
             hidden_states.append(state)
             observations.append(observation)
 
-            for k in torch.arange(1, length-1):
+            for k in torch.arange(1, length-2):
                 transition_p_t = self.generatorConf.transition_prob_t[state]
                 state = pyro.sample("x_{}_{}".format(j, k),
                                     pyro.distributions.Categorical(transition_p_t))
                 
                 hidden_AAs_sequence = self.AA_indices_sequence_to_AA_sequence(hidden_states)
 
                 emission_p_t = self.generatorConf.emission_prob_t[state]
@@ -191,15 +266,20 @@
                         emission_p_t = constraints[self.generatorConf.AAs[state]]
                         break
 
                 observation = pyro.sample("y_{}_{}".format(j, k),
                                           pyro.distributions.Categorical(emission_p_t))
 
                 hidden_states.append(state)
-                observations.append(observation)   
+                observations.append(observation)
+
+            #generate the stop codon
+            state, observation = self.generate_token(Position.STOP)
+            hidden_states.append(state)
+            observations.append(observation)    
 
             AA_sample = torch.Tensor(hidden_states)
             CDs_sample = torch.Tensor(observations)
 
             AAs_samples.append(AA_sample)
             CDs_samples.append(CDs_sample)
```

### Comparing `syncdsgen-0.0.1/LICENCE` & `syncdsgen-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `syncdsgen-0.0.1/pyproject.toml` & `syncdsgen-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "syncdsgen"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ramses TANANKEM", email="tanankemr@gmail.com" },
 ]
 description = "A package to generate synthetic coding sequences data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

