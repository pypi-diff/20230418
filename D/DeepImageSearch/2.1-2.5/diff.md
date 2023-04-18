# Comparing `tmp/DeepImageSearch-2.1.tar.gz` & `tmp/DeepImageSearch-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepImageSearch-2.1.tar", last modified: Sat Apr  8 14:35:26 2023, max compression
+gzip compressed data, was "DeepImageSearch-2.5.tar", last modified: Tue Apr 18 04:23:24 2023, max compression
```

## Comparing `DeepImageSearch-2.1.tar` & `DeepImageSearch-2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 14:35:26.488966 DeepImageSearch-2.1/
-drwxrwxrwx   0        0        0        0 2023-04-08 14:35:26.467946 DeepImageSearch-2.1/DeepImageSearch/
--rw-rw-rw-   0        0        0    10482 2023-04-08 12:09:08.000000 DeepImageSearch-2.1/DeepImageSearch/DeepImageSearch.py
--rw-rw-rw-   0        0        0       72 2023-04-08 12:09:17.000000 DeepImageSearch-2.1/DeepImageSearch/__init__.py
--rw-rw-rw-   0        0        0      197 2023-04-08 07:52:54.000000 DeepImageSearch-2.1/DeepImageSearch/config.py
-drwxrwxrwx   0        0        0        0 2023-04-08 14:35:26.488966 DeepImageSearch-2.1/DeepImageSearch.egg-info/
--rw-rw-rw-   0        0        0     6035 2023-04-08 14:35:26.000000 DeepImageSearch-2.1/DeepImageSearch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-04-08 14:35:26.000000 DeepImageSearch-2.1/DeepImageSearch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 14:35:26.000000 DeepImageSearch-2.1/DeepImageSearch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-08 14:35:26.000000 DeepImageSearch-2.1/DeepImageSearch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-08 14:35:26.000000 DeepImageSearch-2.1/DeepImageSearch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1080 2023-04-08 07:52:54.000000 DeepImageSearch-2.1/LICENSE.txt
--rw-rw-rw-   0        0        0     6035 2023-04-08 14:35:26.488966 DeepImageSearch-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4939 2023-04-08 14:09:14.000000 DeepImageSearch-2.1/README.md
--rw-rw-rw-   0        0        0       87 2023-04-08 14:35:26.488966 DeepImageSearch-2.1/setup.cfg
--rw-rw-rw-   0        0        0     1622 2023-04-08 14:34:59.000000 DeepImageSearch-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 04:23:24.935655 DeepImageSearch-2.5/
+drwxrwxrwx   0        0        0        0 2023-04-18 04:23:24.903613 DeepImageSearch-2.5/DeepImageSearch/
+-rw-rw-rw-   0        0        0    11598 2023-04-18 04:08:02.000000 DeepImageSearch-2.5/DeepImageSearch/DeepImageSearch.py
+-rw-rw-rw-   0        0        0       68 2023-04-17 14:14:49.000000 DeepImageSearch-2.5/DeepImageSearch/__init__.py
+-rw-rw-rw-   0        0        0      411 2023-04-17 14:47:27.000000 DeepImageSearch-2.5/DeepImageSearch/config.py
+drwxrwxrwx   0        0        0        0 2023-04-18 04:23:24.935655 DeepImageSearch-2.5/DeepImageSearch.egg-info/
+-rw-rw-rw-   0        0        0     6580 2023-04-18 04:23:24.000000 DeepImageSearch-2.5/DeepImageSearch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-04-18 04:23:24.000000 DeepImageSearch-2.5/DeepImageSearch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 04:23:24.000000 DeepImageSearch-2.5/DeepImageSearch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-04-18 04:23:24.000000 DeepImageSearch-2.5/DeepImageSearch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-18 04:23:24.000000 DeepImageSearch-2.5/DeepImageSearch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1080 2023-04-08 07:52:54.000000 DeepImageSearch-2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     6580 2023-04-18 04:23:24.935655 DeepImageSearch-2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5427 2023-04-18 03:58:24.000000 DeepImageSearch-2.5/README.md
+-rw-rw-rw-   0        0        0       87 2023-04-18 04:23:24.935655 DeepImageSearch-2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1683 2023-04-18 04:22:31.000000 DeepImageSearch-2.5/setup.py
```

### Comparing `DeepImageSearch-2.1/DeepImageSearch/DeepImageSearch.py` & `DeepImageSearch-2.5/DeepImageSearch/DeepImageSearch.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,265 +1,243 @@
 import DeepImageSearch.config as config
 import os
 import pandas as pd
 import matplotlib.pyplot as plt
 from PIL import Image
 from tqdm import tqdm
 import numpy as np
-from annoy import AnnoyIndex
 from torchvision import transforms
 import torch
-from torchvision.models import vgg16
 from torch.autograd import Variable
 import timm
 from PIL import ImageOps
 import math
+import faiss
 
-class LoadData:
+class Load_Data:
     """A class for loading data from single/multiple folders or a CSV file"""
 
     def __init__(self):
         """
         Initializes an instance of LoadData class
         """
         pass
     
     def from_folder(self, folder_list: list):
         """
-        Method to load data from a single folder path or a list of folder paths
+        Adds images from the specified folders to the image_list.
 
-        Args:
-        - folder_list (list): A list of folder paths
-
-        Returns:
-        - image_path (list): A list of image paths
+        Parameters:
+        -----------
+        folder_list : list
+            A list of paths to the folders containing images to be added to the image_list.
         """
         self.folder_list = folder_list
         image_path = []
         for folder in self.folder_list:
-            for path in os.listdir(folder):
-                image_path.append(os.path.join(folder, path))
+            for root, dirs, files in os.walk(folder):
+                for file in files:
+                    if file.lower().endswith(('.png', '.jpg', '.jpeg', '.gif', '.bmp')):
+                        image_path.append(os.path.join(root, file))
         return image_path
 
     def from_csv(self, csv_file_path: str, images_column_name: str):
         """
-        Method to load data from a CSV file with a column containing image paths
+        Adds images from the specified column of a CSV file to the image_list.
 
-        Args:
-        - csv_file_path (str): The path of the CSV file
-        - images_column_name (str): The name of the column containing the image paths
-
-        Returns:
-        - image_path (list): A list of image paths
+        Parameters:
+        -----------
+        csv_file_path : str
+            The path to the CSV file.
+        images_column_name : str
+            The name of the column containing the paths to the images to be added to the image_list.
         """
         self.csv_file_path = csv_file_path
         self.images_column_name = images_column_name
         return pd.read_csv(self.csv_file_path)[self.images_column_name].to_list()
 
-class FeatureExtractor:
-    """A class for extracting features using a transformer-based feature extraction model"""
-
-    def __init__(self, model_name='vit_base_patch16_224', pretrained=True):
+class Search_Setup:
+    """ A class for setting up and running image similarity search."""
+    def __init__(self, image_list: list, model_name='vgg19', pretrained=True, image_count: int = None):
         """
-        Initializes an instance of FeatureExtractor class
-
-        Args:
-        - model_name (str): The name of the pre-trained model to use for feature extraction
-        - pretrained (bool): Whether to use the pre-trained weights or not
+        Parameters:
+        -----------
+        image_list : list
+        A list of images to be indexed and searched.
+        model_name : str, optional (default='vgg19')
+        The name of the pre-trained model to use for feature extraction.
+        pretrained : bool, optional (default=True)
+        Whether to use the pre-trained weights for the chosen model.
+        image_count : int, optional (default=None)
+        The number of images to be indexed and searched. If None, all images in the image_list will be used.
         """
         self.model_name = model_name
         self.pretrained = pretrained
-        
+        self.image_data = pd.DataFrame()
+        self.d = None
+        if image_count==None:
+            self.image_list = image_list
+        else:
+            self.image_list = image_list[:image_count]
+
+        if f'metadata-files/{self.model_name}' not in os.listdir():
+            try:
+                os.makedirs(f'metadata-files/{self.model_name}')
+            except Exception as e:
+                pass
+                #print(f'\033[91m file already exists: metadata-files/{self.model_name}')
+
         # Load the pre-trained model and remove the last layer
+        print("\033[91m Please Wait Model Is Loading or Downloading From Server!")
         base_model = timm.create_model(self.model_name, pretrained=self.pretrained)
         self.model = torch.nn.Sequential(*list(base_model.children())[:-1])
         self.model.eval()
+        print(f"\033[92m Model Loaded Successfully: {model_name}")
 
-    def extract(self, img):
-        """
-        Method to extract features from an image using the pre-trained model
-
-        Args:
-        - img (PIL Image): The input image
-
-        Returns:
-        - feature (numpy array): The extracted features
-        """
+    def _extract(self, img):
         # Resize and convert the image
         img = img.resize((224, 224))
         img = img.convert('RGB')
-        
+
         # Preprocess the image
         preprocess = transforms.Compose([
             transforms.ToTensor(),
-            transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]),
+            transforms.Normalize(mean=[0.485, 0.456, 0.406],std=[0.229,0.224, 0.225]),
         ])
         x = preprocess(img)
         x = Variable(torch.unsqueeze(x, dim=0).float(), requires_grad=False)
-        
+
         # Extract features
         feature = self.model(x)
         feature = feature.data.numpy().flatten()
         return feature / np.linalg.norm(feature)
 
-    def get_feature(self, image_data: list):
-        """
-        Method to extract features from a list of image paths
-
-        Args:
-        - image_data (list): A list of image paths
-
-        Returns:
-        - features (list): A list of extracted features
-        """
+    def _get_feature(self, image_data: list):
         self.image_data = image_data
         features = []
         for img_path in tqdm(self.image_data):  # Iterate through images
             # Extract features from the image
             try:
-                feature = self.extract(img=Image.open(img_path))
+                feature = self._extract(img=Image.open(img_path))
                 features.append(feature)
             except:
-                # If there is an error, append None to the feature list
-                features.append(None)
-                continue
+               # If there is an error, append None to the feature list
+               features.append(None)
+               continue
         return features
-    
-class Index:
-    def __init__(self, image_list: list):
-        """
-        Initializes the Index class with a list of image paths.
-
-        Parameters
-        ----------
-        image_list : list
-            A list of image paths.
-        """
-        self.image_list = image_list
-        if 'meta-data-files' not in os.listdir():
-            os.makedirs("meta-data-files")
-        self.FE = FeatureExtractor()
 
-    def start_feature_extraction(self):
-        """
-        Extracts features from images and saves the data as a pickle file.
-
-        Returns
-        -------
-        image_data : DataFrame
-            A DataFrame containing image paths and their extracted features.
-        """
+    def _start_feature_extraction(self):
         image_data = pd.DataFrame()
         image_data['images_paths'] = self.image_list
-        f_data = self.FE.get_feature(self.image_list)
-        image_data['features']  = f_data
+        f_data = self._get_feature(self.image_list)
+        image_data['features'] = f_data
         image_data = image_data.dropna().reset_index(drop=True)
-        image_data.to_pickle(config.image_data_with_features_pkl)
-        print("Image Meta Information Saved: [meta-data-files/image_data_features.pkl]")
+        image_data.to_pickle(config.image_data_with_features_pkl(self.model_name))
+        print(f"\033[94m Image Meta Information Saved: [metadata-files/{self.model_name}/image_data_features.pkl]")
         return image_data
 
-    def start_indexing(self, image_data):
-        """
-        Indexes the extracted image features using Annoy.
-
-        Parameters
-        ----------
-        image_data : DataFrame
-            A DataFrame containing image paths and their extracted features.
-        """
+    def _start_indexing(self, image_data):
         self.image_data = image_data
-        f = len(image_data['features'][0]) # Length of item vector that will be indexed
-        t = AnnoyIndex(f, 'euclidean')
-        for i, v in tqdm(zip(self.image_data.index, image_data['features'])):
-            t.add_item(i, v)
-        t.build(100) # 100 trees
-        print("Saved the Indexed File:"+"[meta-data-files/image_features_vectors.ann]")
-        t.save(config.image_features_vectors_ann)
-
-    def start(self):
-        """
-        Starts the feature extraction and indexing process.
-        """
-        if len(os.listdir("meta-data-files/")) == 0:
-            data = self.start_feature_extraction()
-            self.start_indexing(data)
+        d = len(image_data['features'][0])  # Length of item vector that will be indexed
+        self.d = d
+        index = faiss.IndexFlatL2(d)
+        features_matrix = np.vstack(image_data['features'].values).astype(np.float32)
+        index.add(features_matrix)  # Add the features matrix to the index
+        faiss.write_index(index, config.image_features_vectors_idx(self.model_name))
+        print("\033[94m Saved The Indexed File:" + f"[metadata-files/{self.model_name}/image_features_vectors.idx]")
+
+    def run_index(self):
+        """
+        Indexes the images in the image_list and creates an index file for fast similarity search.
+        """
+        if len(os.listdir(f'metadata-files/{self.model_name}')) == 0:
+            data = self._start_feature_extraction()
+            self._start_indexing(data)
         else:
-            print("Metadata and Features are already present, Do you want Extract Again? Enter yes or no")
-            flag  = str(input())
+            print("\033[91m Metadata and Features are already present, Do you want Extract Again? Enter yes or no")
+            flag = str(input())
             if flag.lower() == 'yes':
-                data = self.start_feature_extraction()
-                self.start_indexing(data)
+                data = self._start_feature_extraction()
+                self._start_indexing(data)
             else:
-                print("Meta data already Present, Please Apply Search!")
-                print(os.listdir("meta-data-files/"))
+                print("\033[93m Meta data already Present, Please Apply Search!")
+                print(os.listdir(f'metadata-files/{self.model_name}'))
+        self.image_data = pd.read_pickle(config.image_data_with_features_pkl(self.model_name))
+        self.f = len(self.image_data['features'][0])
 
-class SearchImage:
-    def __init__(self):
+    def add_images_to_index(self, new_image_paths: list):
         """
-        Initialize the `SearchImage` class.
+        Adds new images to the existing index.
 
-        Attributes:
-            image_data (pandas.DataFrame): A DataFrame containing the image paths and features.
-            f (int): The length of the feature vectors.
+        Parameters:
+        -----------
+        new_image_paths : list
+            A list of paths to the new images to be added to the index.
         """
-        self.image_data = pd.read_pickle(config.image_data_with_features_pkl)
-        self.f = len(self.image_data['features'][0])
+        # Load existing metadata and index
+        self.image_data = pd.read_pickle(config.image_data_with_features_pkl(self.model_name))
+        index = faiss.read_index(config.image_features_vectors_idx(self.model_name))
 
-    def search_by_vector(self, v, n: int):
-        """
-        Search for similar images using a given feature vector.
+        for new_image_path in tqdm(new_image_paths):
+            # Extract features from the new image
+            try:
+                img = Image.open(new_image_path)
+                feature = self._extract(img)
+            except Exception as e:
+                print(f"\033[91m Error extracting features from the new image: {e}")
+                continue
 
-        Args:
-            v (numpy.ndarray): The feature vector to search by.
-            n (int): The number of similar images to retrieve.
+            # Add the new image to the metadata
+            new_metadata = pd.DataFrame({"images_paths": [new_image_path], "features": [feature]})
+            #self.image_data = self.image_data.append(new_metadata, ignore_index=True)
+            self.image_data  =pd.concat([self.image_data, new_metadata], axis=0, ignore_index=True)
 
-        Returns:
-            dict: A dictionary mapping the indices of the most similar images to their corresponding image paths.
-        """
-        self.v = v
-        self.n = n
-        u = AnnoyIndex(self.f, 'euclidean')
-        u.load(config.image_features_vectors_ann)
-        index_list = u.get_nns_by_vector(self.v, self.n)
-        return dict(zip(index_list, self.image_data.iloc[index_list]['images_paths'].to_list()))
+            # Add the new image to the index
+            index.add(np.array([feature], dtype=np.float32))
 
-    def get_query_vector(self, image_path: str):
-        """
-        Extract the feature vector for a given image.
+        # Save the updated metadata and index
+        self.image_data.to_pickle(config.image_data_with_features_pkl(self.model_name))
+        faiss.write_index(index, config.image_features_vectors_idx(self.model_name))
 
-        Args:
-            image_path (str): The path to the image file.
+        print(f"\033[92m New images added to the index: {len(new_image_paths)}")
 
-        Returns:
-            numpy.ndarray: The feature vector for the image.
-        """
+    def _search_by_vector(self, v, n: int):
+        self.v = v
+        self.n = n
+        index = faiss.read_index(config.image_features_vectors_idx(self.model_name))
+        D, I = index.search(np.array([self.v], dtype=np.float32), self.n)
+        return dict(zip(I[0], self.image_data.iloc[I[0]]['images_paths'].to_list()))
+
+    def _get_query_vector(self, image_path: str):
         self.image_path = image_path
         img = Image.open(self.image_path)
-        fe = FeatureExtractor()
-        query_vector = fe.extract(img)
+        query_vector = self._extract(img)
         return query_vector
 
     def plot_similar_images(self, image_path: str, number_of_images: int = 6):
         """
-        Display a plot of the input image and its most similar images.
+        Plots a given image and its most similar images according to the indexed image features.
 
-        Args:
-            image_path (str): The path to the input image file.
-            number_of_images (int): The number of similar images to display.
+        Parameters:
+        -----------
+        image_path : str
+            The path to the query image to be plotted.
+        number_of_images : int, optional (default=6)
+            The number of most similar images to the query image to be plotted.
         """
         input_img = Image.open(image_path)
         input_img_resized = ImageOps.fit(input_img, (224, 224), Image.LANCZOS)
         plt.figure(figsize=(5, 5))
         plt.axis('off')
         plt.title('Input Image', fontsize=18)
         plt.imshow(input_img_resized)
         plt.show()
 
-        query_vector = self.get_query_vector(image_path)
-        img_list = list(self.search_by_vector(query_vector, number_of_images).values())
+        query_vector = self._get_query_vector(image_path)
+        img_list = list(self._search_by_vector(query_vector, number_of_images).values())
 
         grid_size = math.ceil(math.sqrt(number_of_images))
         axes = []
         fig = plt.figure(figsize=(20, 15))
         for a in range(number_of_images):
             axes.append(fig.add_subplot(grid_size, grid_size, a + 1))
             plt.axis('off')
@@ -267,23 +245,34 @@
             img_resized = ImageOps.fit(img, (224, 224), Image.LANCZOS)
             plt.imshow(img_resized)
         fig.tight_layout()
         fig.subplots_adjust(top=0.93)
         fig.suptitle('Similar Result Found', fontsize=22)
         plt.show(fig)
 
-    def get_similar_images(self,image_path:str,number_of_images:int=10):
+    def get_similar_images(self, image_path: str, number_of_images: int = 10):
         """
-        Retrieve a dictionary of the most similar images to the input image.
-
-        Args:
-            image_path (str): The path to the input image file.
-            number_of_images (int): The number of similar images to retrieve.
+        Returns the most similar images to a given query image according to the indexed image features.
 
-        Returns:
-            dict: A dictionary mapping the indices of the most similar images to their corresponding image paths.
+        Parameters:
+        -----------
+        image_path : str
+            The path to the query image.
+        number_of_images : int, optional (default=10)
+            The number of most similar images to the query image to be returned.
         """
         self.image_path = image_path
         self.number_of_images = number_of_images
-        query_vector = self.get_query_vector(self.image_path)
-        img_dict = self.search_by_vector(query_vector,self.number_of_images)
-        return img_dict
+        query_vector = self._get_query_vector(self.image_path)
+        img_dict = self._search_by_vector(query_vector, self.number_of_images)
+        return img_dict
+    def get_image_metadata_file(self):
+        """
+        Returns the metadata file containing information about the indexed images.
+
+        Returns:
+        --------
+        DataFrame
+            The Panda DataFrame of the metadata file.
+        """
+        self.image_data = pd.read_pickle(config.image_data_with_features_pkl(self.model_name))
+        return self.image_data
```

### Comparing `DeepImageSearch-2.1/DeepImageSearch.egg-info/PKG-INFO` & `DeepImageSearch-2.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,79 @@
-Metadata-Version: 2.1
-Name: DeepImageSearch
-Version: 2.1
-Summary: Deep Image Search is an AI-based image search engine that incorporates ViT (Vision Transformer) for feature extraction and utilizes a tree-based vectorized search technique.
-Home-page: https://github.com/TechyNilesh/DeepImageSearch
-Author: Nilesh Verma
-Author-email: me@nileshverma.com
-License: MIT
-Download-URL: https://github.com/TechyNilesh/DeepImageSearch/archive/refs/tags/v_20.tar.gz
-Keywords: Deep Image Search Engine,AI Image search,Image Search Python
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Deep Image Search - AI-Based Image Search Engine
 <p align="center"><img src="https://raw.githubusercontent.com/TechyNilesh/DeepImageSearch/786e96c48561d67be47dccbab2bc8debced414a3/images/deep%20image%20search%20logo%20New.png" alt="Deep+Image+Search+logo" height="218" width="350"></p>
 
-**Deep Image Search** is an AI-based image search engine that incorporates **ViT (Vision Transformer)** for feature extraction and utilizes a **tree-based vectorized search** technique.
+**DeepImageSearch** is a powerful Python library that combines **state-of-the-art computer vision models** for feature extraction with **highly optimized algorithms for indexing and searching**. This enables fast and accurate similarity search and clustering of dense vectors, allowing users to build **scalable image search systems** capable of handling large-scale datasets. The library offers seamless integration with Python and provides **GPU support** for accelerated processing, delivering a comprehensive solution for researchers and developers working on image-based search and retrieval applications. By incorporating the **Vision Transformer (ViT) model**, DeepImageSearch further enhances its capabilities in identifying and understanding complex image patterns, making it an essential tool for advanced image search and analysis tasks.
 
 ![Generic badge](https://img.shields.io/badge/AI-Advance-green.svg) ![Generic badge](https://img.shields.io/badge/Python-v3-blue.svg) ![Generic badge](https://img.shields.io/badge/pip-v3-red.svg)
-![Generic badge](https://img.shields.io/badge/ViT-Vision_Transformer-g.svg)   ![Generic badge](https://img.shields.io/badge/TorchVision-v0.15-orange.svg) ![Generic badge](https://img.shields.io/badge/Annoy-latest-green.svg) [![Downloads](https://static.pepy.tech/personalized-badge/deepimagesearch?period=total&units=none&left_color=grey&right_color=green&left_text=Downloads)](https://pepy.tech/project/deepimagesearch)
+![Generic badge](https://img.shields.io/badge/ViT-Vision_Transformer-g.svg)   ![Generic badge](https://img.shields.io/badge/TorchVision-v0.15-orange.svg) ![Generic badge](https://img.shields.io/badge/FAISS-latest-green.svg) [![Downloads](https://static.pepy.tech/personalized-badge/deepimagesearch?period=total&units=none&left_color=grey&right_color=green&left_text=Downloads)](https://pepy.tech/project/deepimagesearch)
 
 ## Developed By
 
 ### [Nilesh Verma](https://nileshverma.com "Nilesh Verma")
 
 ## Features
-- Faster Search **O(logN)** Complexity.
-- High Accurate Output Result.
-- Best for Implementing on python based web application or APIs.
-- Best implementation for College students and freshers for project creation.
-- Applications are Images based E-commerce recommendation, Social media and other image-based platforms that want to implement image recommendation and search.
+- You can now load more than 500+ pre-trained state-of-the-art computer vision models available on [timm](https://timm.fast.ai/).
+- Faster Search using [FAISS (Facebook AI Similarity Search)](https://github.com/facebookresearch/faiss).
+- Highly Accurate Output Results.
+- GPU & CPU based indexing and Searching Support.
+- Best for implementing on Python-based web applications or APIs.
+- Applications include image-based e-commerce recommendations, social media, and other image-based platforms that want to implement image recommendations and search.
 
 ## Installation
 
 This library is compatible with both *windows* and *Linux system* you can just use **PIP command** to install this library on your system:
 
 ```shell
-pip install DeepImageSearch
+pip install DeepImageSearch --upgrade
 ```
-
-If you are facing any VS C++ 14 related issue in windows during installation, kindly refer to following solution: [Pip error: Microsoft Visual C++ 14.0 is required](https://stackoverflow.com/questions/44951456/pip-error-microsoft-visual-c-14-0-is-required "Pip error: Microsoft Visual C++ 14.0 is required")
+<span style="color:yellow">  If you're using a GPU, first uninstall the **faiss_cpu** version and then try installing the **faiss_gpu** version. The library installs the CPU version by default because not all systems support GPUs. </span>
 
 ## How To Use?
 
 We have provided the **Demo** folder under the *GitHub repository*, you can find the example in both **.py** and **.ipynb**  file. Following are the ideal flow of the code:
 
-### 1. Importing the Important Classes
-There are three important classes you need to load **LoadData** - for data loading, **Index** - for indexing the images to database/folder, **SearchImage** - For searching and Plotting the images
-
 ```python
-# Importing the proper classes
-from DeepImageSearch import Index,LoadData,SearchImage
-```
+from DeepImageSearch import Load_Data, Search_Setup
 
-### 2. Loading the Images Data
+# Load images from a folder
+image_list = Load_Data().from_folder(['folder_path'])
 
-For loading the images data we need to use the **LoadData** object, from there we can import images from the CSV file and Single/Multiple Folders.
+ # Set up the search engine, You can load 'vit_base_patch16_224_in21k', 'resnet50' etc more then 500+ models 
+ st = Search_Setup(image_list=image_list, model_name='vgg19', pretrained=True, image_count=100)
 
-```python
-# load the Images from the Folder (You can also import data from multiple folders in python list type)
-image_list = LoadData().from_folder(['images','wiki-images'])
-# Load data from CSV file
-image_list = LoadData().from_csv(csv_file_path='your_csv_file.csv',images_column_name='column_name')
-```
-### 3. Indexing and Saving The File in Local Folder
+# Index the images
+st.run_index()
 
-For faster retrieval we are using tree-based indexing techniques for Images features, So for that, we need to store meta-information on the local path **[meta-data-files/]** folder.
+# Get metadata
+metadata = st.get_image_metadata_file()
 
-```python
-# For Faster Serching we need to index Data first, After Indexing all the meta data stored on the local path
-Index(image_list).start()
-```
-### 3. Searching
+# Add new images to the index
+st.add_images_to_index(['image_path_1', 'image_path_2'])
 
-Searching operation is performed by the following method:
+# Get similar images
+st.get_similar_images(image_path='image_path', number_of_images=10)
 
-```python
-# for searching, you need to give the image path and the number of the similar image you want
-SearchImage().get_similar_images(image_path=image_list[0],number_of_images=5)
-```
-you can also plot some similar images for viewing purpose by following the code method:
+# Plot similar images
+st.plot_similar_images(image_path='image_path', number_of_images=9)
 
-```python
-# If you want to plot similar images you can use this method, It will plot 6 most similar images from the data index
-SearchImage().plot_similar_images(image_path = image_list[0],number_of_images=6)
+# Update metadata
+metadata = st.get_image_metadata_file()
 ```
+
+This code demonstrates how to load images, set up the search engine, index the images, add new images to the index, and retrieve similar images.
+
+<span style="color:red"> **Note:** Some models may not work properly due to resizing and normalization issues. By default, I have chosen a size of 224x244. Please try to select models that support this size or resized inputs. I have already tested many models, but testing over 500 is beyond my scope.</span>
+
+## Documentation
+
+This project aims to provide a powerful image search engine using deep learning techniques. To get started, please follow the link: [Read Full Documents](https://github.com/TechyNilesh/DeepImageSearch/blob/main/Documents/Document.md)
+
 ## Screenshot
 
-<p align="center"><img src="https://raw.githubusercontent.com/TechyNilesh/DeepImageSearch/786e96c48561d67be47dccbab2bc8debced414a3/images/Deep-Image-Search-Demo-Screenshot.png?" alt="Brain+Machine" height="auto" width="auto"></p>
+<p align="center"><img src="https://github.com/TechyNilesh/DeepImageSearch/blob/c2a5e511662adade6ddece9be67167fe3f96cc4c/images/Deep-Image-Search-Demo-Screenshot.png?raw=true" alt="Brain+Machine" height="auto" width="auto"></p>
 
 ## Citaion
 
 If you use DeepImageSerach in your Research/Product, please cite the following GitHub Repository:
 
 ```latex
 @misc{TechyNilesh/DeepImageSearch,
@@ -112,9 +85,7 @@
   howpublished = {\url{https://github.com/TechyNilesh/DeepImageSearch}},
 }
 ```
 
 ### Please do STAR the repository, if it helped you in anyway.
 
 **More cool features will be added in future. Feel free to give suggestions, report bugs and contribute.**
-
-
```

### Comparing `DeepImageSearch-2.1/LICENSE.txt` & `DeepImageSearch-2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DeepImageSearch-2.1/PKG-INFO` & `DeepImageSearch-2.5/DeepImageSearch.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: DeepImageSearch
-Version: 2.1
-Summary: Deep Image Search is an AI-based image search engine that incorporates ViT (Vision Transformer) for feature extraction and utilizes a tree-based vectorized search technique.
+Version: 2.5
+Summary: DeepImageSearch is a Python library for fast and accurate image search. It offers seamless integration with Python, GPU support, and advanced capabilities for identifying complex image patterns using the Vision Transformer models.
 Home-page: https://github.com/TechyNilesh/DeepImageSearch
 Author: Nilesh Verma
 Author-email: me@nileshverma.com
 License: MIT
-Download-URL: https://github.com/TechyNilesh/DeepImageSearch/archive/refs/tags/v_20.tar.gz
+Download-URL: https://github.com/TechyNilesh/DeepImageSearch/archive/refs/tags/v_25.tar.gz
 Keywords: Deep Image Search Engine,AI Image search,Image Search Python
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,87 +20,83 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Deep Image Search - AI-Based Image Search Engine
 <p align="center"><img src="https://raw.githubusercontent.com/TechyNilesh/DeepImageSearch/786e96c48561d67be47dccbab2bc8debced414a3/images/deep%20image%20search%20logo%20New.png" alt="Deep+Image+Search+logo" height="218" width="350"></p>
 
-**Deep Image Search** is an AI-based image search engine that incorporates **ViT (Vision Transformer)** for feature extraction and utilizes a **tree-based vectorized search** technique.
+**DeepImageSearch** is a powerful Python library that combines **state-of-the-art computer vision models** for feature extraction with **highly optimized algorithms for indexing and searching**. This enables fast and accurate similarity search and clustering of dense vectors, allowing users to build **scalable image search systems** capable of handling large-scale datasets. The library offers seamless integration with Python and provides **GPU support** for accelerated processing, delivering a comprehensive solution for researchers and developers working on image-based search and retrieval applications. By incorporating the **Vision Transformer (ViT) model**, DeepImageSearch further enhances its capabilities in identifying and understanding complex image patterns, making it an essential tool for advanced image search and analysis tasks.
 
 ![Generic badge](https://img.shields.io/badge/AI-Advance-green.svg) ![Generic badge](https://img.shields.io/badge/Python-v3-blue.svg) ![Generic badge](https://img.shields.io/badge/pip-v3-red.svg)
-![Generic badge](https://img.shields.io/badge/ViT-Vision_Transformer-g.svg)   ![Generic badge](https://img.shields.io/badge/TorchVision-v0.15-orange.svg) ![Generic badge](https://img.shields.io/badge/Annoy-latest-green.svg) [![Downloads](https://static.pepy.tech/personalized-badge/deepimagesearch?period=total&units=none&left_color=grey&right_color=green&left_text=Downloads)](https://pepy.tech/project/deepimagesearch)
+![Generic badge](https://img.shields.io/badge/ViT-Vision_Transformer-g.svg)   ![Generic badge](https://img.shields.io/badge/TorchVision-v0.15-orange.svg) ![Generic badge](https://img.shields.io/badge/FAISS-latest-green.svg) [![Downloads](https://static.pepy.tech/personalized-badge/deepimagesearch?period=total&units=none&left_color=grey&right_color=green&left_text=Downloads)](https://pepy.tech/project/deepimagesearch)
 
 ## Developed By
 
 ### [Nilesh Verma](https://nileshverma.com "Nilesh Verma")
 
 ## Features
-- Faster Search **O(logN)** Complexity.
-- High Accurate Output Result.
-- Best for Implementing on python based web application or APIs.
-- Best implementation for College students and freshers for project creation.
-- Applications are Images based E-commerce recommendation, Social media and other image-based platforms that want to implement image recommendation and search.
+- You can now load more than 500+ pre-trained state-of-the-art computer vision models available on [timm](https://timm.fast.ai/).
+- Faster Search using [FAISS (Facebook AI Similarity Search)](https://github.com/facebookresearch/faiss).
+- Highly Accurate Output Results.
+- GPU & CPU based indexing and Searching Support.
+- Best for implementing on Python-based web applications or APIs.
+- Applications include image-based e-commerce recommendations, social media, and other image-based platforms that want to implement image recommendations and search.
 
 ## Installation
 
 This library is compatible with both *windows* and *Linux system* you can just use **PIP command** to install this library on your system:
 
 ```shell
-pip install DeepImageSearch
+pip install DeepImageSearch --upgrade
 ```
-
-If you are facing any VS C++ 14 related issue in windows during installation, kindly refer to following solution: [Pip error: Microsoft Visual C++ 14.0 is required](https://stackoverflow.com/questions/44951456/pip-error-microsoft-visual-c-14-0-is-required "Pip error: Microsoft Visual C++ 14.0 is required")
+<span style="color:yellow">  If you're using a GPU, first uninstall the **faiss_cpu** version and then try installing the **faiss_gpu** version. The library installs the CPU version by default because not all systems support GPUs. </span>
 
 ## How To Use?
 
 We have provided the **Demo** folder under the *GitHub repository*, you can find the example in both **.py** and **.ipynb**  file. Following are the ideal flow of the code:
 
-### 1. Importing the Important Classes
-There are three important classes you need to load **LoadData** - for data loading, **Index** - for indexing the images to database/folder, **SearchImage** - For searching and Plotting the images
-
 ```python
-# Importing the proper classes
-from DeepImageSearch import Index,LoadData,SearchImage
-```
+from DeepImageSearch import Load_Data, Search_Setup
 
-### 2. Loading the Images Data
+# Load images from a folder
+image_list = Load_Data().from_folder(['folder_path'])
 
-For loading the images data we need to use the **LoadData** object, from there we can import images from the CSV file and Single/Multiple Folders.
+ # Set up the search engine, You can load 'vit_base_patch16_224_in21k', 'resnet50' etc more then 500+ models 
+ st = Search_Setup(image_list=image_list, model_name='vgg19', pretrained=True, image_count=100)
 
-```python
-# load the Images from the Folder (You can also import data from multiple folders in python list type)
-image_list = LoadData().from_folder(['images','wiki-images'])
-# Load data from CSV file
-image_list = LoadData().from_csv(csv_file_path='your_csv_file.csv',images_column_name='column_name')
-```
-### 3. Indexing and Saving The File in Local Folder
+# Index the images
+st.run_index()
 
-For faster retrieval we are using tree-based indexing techniques for Images features, So for that, we need to store meta-information on the local path **[meta-data-files/]** folder.
+# Get metadata
+metadata = st.get_image_metadata_file()
 
-```python
-# For Faster Serching we need to index Data first, After Indexing all the meta data stored on the local path
-Index(image_list).start()
-```
-### 3. Searching
+# Add new images to the index
+st.add_images_to_index(['image_path_1', 'image_path_2'])
 
-Searching operation is performed by the following method:
+# Get similar images
+st.get_similar_images(image_path='image_path', number_of_images=10)
 
-```python
-# for searching, you need to give the image path and the number of the similar image you want
-SearchImage().get_similar_images(image_path=image_list[0],number_of_images=5)
-```
-you can also plot some similar images for viewing purpose by following the code method:
+# Plot similar images
+st.plot_similar_images(image_path='image_path', number_of_images=9)
 
-```python
-# If you want to plot similar images you can use this method, It will plot 6 most similar images from the data index
-SearchImage().plot_similar_images(image_path = image_list[0],number_of_images=6)
+# Update metadata
+metadata = st.get_image_metadata_file()
 ```
+
+This code demonstrates how to load images, set up the search engine, index the images, add new images to the index, and retrieve similar images.
+
+<span style="color:red"> **Note:** Some models may not work properly due to resizing and normalization issues. By default, I have chosen a size of 224x244. Please try to select models that support this size or resized inputs. I have already tested many models, but testing over 500 is beyond my scope.</span>
+
+## Documentation
+
+This project aims to provide a powerful image search engine using deep learning techniques. To get started, please follow the link: [Read Full Documents](https://github.com/TechyNilesh/DeepImageSearch/blob/main/Documents/Document.md)
+
 ## Screenshot
 
-<p align="center"><img src="https://raw.githubusercontent.com/TechyNilesh/DeepImageSearch/786e96c48561d67be47dccbab2bc8debced414a3/images/Deep-Image-Search-Demo-Screenshot.png?" alt="Brain+Machine" height="auto" width="auto"></p>
+<p align="center"><img src="https://github.com/TechyNilesh/DeepImageSearch/blob/c2a5e511662adade6ddece9be67167fe3f96cc4c/images/Deep-Image-Search-Demo-Screenshot.png?raw=true" alt="Brain+Machine" height="auto" width="auto"></p>
 
 ## Citaion
 
 If you use DeepImageSerach in your Research/Product, please cite the following GitHub Repository:
 
 ```latex
 @misc{TechyNilesh/DeepImageSearch,
```

