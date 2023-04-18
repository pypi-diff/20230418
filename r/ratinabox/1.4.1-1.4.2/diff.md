# Comparing `tmp/ratinabox-1.4.1.tar.gz` & `tmp/ratinabox-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratinabox-1.4.1.tar", last modified: Tue Apr 11 17:41:30 2023, max compression
+gzip compressed data, was "ratinabox-1.4.2.tar", last modified: Tue Apr 18 10:51:10 2023, max compression
```

## Comparing `ratinabox-1.4.1.tar` & `ratinabox-1.4.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 17:41:30.257229 ratinabox-1.4.1/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.4.1/LICENSE
--rw-r--r--   0 tomgeorge   (501) staff       (20)    25185 2023-04-11 17:41:30.257382 ratinabox-1.4.1/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)    24491 2023-04-11 13:27:49.000000 ratinabox-1.4.1/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.4.1/pyproject.toml
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 17:41:30.250123 ratinabox-1.4.1/ratinabox/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    41124 2023-04-11 16:33:06.000000 ratinabox-1.4.1/ratinabox/Agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    31857 2023-04-06 16:54:27.000000 ratinabox-1.4.1/ratinabox/Environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    80087 2023-04-11 15:07:26.000000 ratinabox-1.4.1/ratinabox/Neurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.4.1/ratinabox/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3820 2023-04-06 16:54:27.000000 ratinabox-1.4.1/ratinabox/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 17:41:30.251946 ratinabox-1.4.1/ratinabox/contribs/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     8793 2023-04-04 15:34:22.000000 ratinabox-1.4.1/ratinabox/contribs/FieldOfViewNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     5777 2023-03-07 14:34:45.000000 ratinabox-1.4.1/ratinabox/contribs/PhasePrecessingPlaceCells.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3913 2023-03-07 14:34:45.000000 ratinabox-1.4.1/ratinabox/contribs/PlaneWaveNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.4.1/ratinabox/contribs/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.4.1/ratinabox/contribs/STDPFeedForwardLayer.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    15009 2023-04-11 17:03:00.000000 ratinabox-1.4.1/ratinabox/contribs/ThetaSequenceAgent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7262 2023-04-10 20:56:43.000000 ratinabox-1.4.1/ratinabox/contribs/ValueNeuron.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.4.1/ratinabox/contribs/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 17:41:30.252972 ratinabox-1.4.1/ratinabox/data/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.4.1/ratinabox/data/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.4.1/ratinabox/data/__init__.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.4.1/ratinabox/data/rat.png
--rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.4.1/ratinabox/data/sargolini.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.4.1/ratinabox/data/tanni.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)    30579 2023-04-11 17:15:32.000000 ratinabox-1.4.1/ratinabox/utils.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 17:41:30.250855 ratinabox-1.4.1/ratinabox.egg-info/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    25185 2023-04-11 17:41:30.000000 ratinabox-1.4.1/ratinabox.egg-info/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)      867 2023-04-11 17:41:30.000000 ratinabox-1.4.1/ratinabox.egg-info/SOURCES.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-11 17:41:30.000000 ratinabox-1.4.1/ratinabox.egg-info/dependency_links.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       46 2023-04-11 17:41:30.000000 ratinabox-1.4.1/ratinabox.egg-info/requires.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-04-11 17:41:30.000000 ratinabox-1.4.1/ratinabox.egg-info/top_level.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)      930 2023-04-11 17:41:30.257745 ratinabox-1.4.1/setup.cfg
--rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.4.1/setup.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-11 17:41:30.257054 ratinabox-1.4.1/tests/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-01-09 16:43:43.000000 ratinabox-1.4.1/tests/test_advanced.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.4.1/tests/test_agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.4.1/tests/test_environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.4.1/tests/test_neurons.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-18 10:51:10.488671 ratinabox-1.4.2/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.4.2/LICENSE
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    25321 2023-04-18 10:51:10.488791 ratinabox-1.4.2/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    24627 2023-04-11 18:06:50.000000 ratinabox-1.4.2/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.4.2/pyproject.toml
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-18 10:51:10.478964 ratinabox-1.4.2/ratinabox/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    41124 2023-04-11 16:33:06.000000 ratinabox-1.4.2/ratinabox/Agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    31857 2023-04-06 16:54:27.000000 ratinabox-1.4.2/ratinabox/Environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    80397 2023-04-17 13:49:59.000000 ratinabox-1.4.2/ratinabox/Neurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.4.2/ratinabox/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3820 2023-04-06 16:54:27.000000 ratinabox-1.4.2/ratinabox/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-18 10:51:10.481601 ratinabox-1.4.2/ratinabox/contribs/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     8793 2023-04-04 15:34:22.000000 ratinabox-1.4.2/ratinabox/contribs/FieldOfViewNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     5777 2023-03-07 14:34:45.000000 ratinabox-1.4.2/ratinabox/contribs/PhasePrecessingPlaceCells.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3913 2023-03-07 14:34:45.000000 ratinabox-1.4.2/ratinabox/contribs/PlaneWaveNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.4.2/ratinabox/contribs/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.4.2/ratinabox/contribs/STDPFeedForwardLayer.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    15009 2023-04-11 17:03:00.000000 ratinabox-1.4.2/ratinabox/contribs/ThetaSequenceAgent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7262 2023-04-10 20:56:43.000000 ratinabox-1.4.2/ratinabox/contribs/ValueNeuron.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.4.2/ratinabox/contribs/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-18 10:51:10.483536 ratinabox-1.4.2/ratinabox/data/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.4.2/ratinabox/data/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.4.2/ratinabox/data/__init__.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.4.2/ratinabox/data/rat.png
+-rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.4.2/ratinabox/data/sargolini.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.4.2/ratinabox/data/tanni.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    30579 2023-04-17 12:58:07.000000 ratinabox-1.4.2/ratinabox/utils.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-18 10:51:10.479894 ratinabox-1.4.2/ratinabox.egg-info/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    25321 2023-04-18 10:51:10.000000 ratinabox-1.4.2/ratinabox.egg-info/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      867 2023-04-18 10:51:10.000000 ratinabox-1.4.2/ratinabox.egg-info/SOURCES.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-18 10:51:10.000000 ratinabox-1.4.2/ratinabox.egg-info/dependency_links.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       46 2023-04-18 10:51:10.000000 ratinabox-1.4.2/ratinabox.egg-info/requires.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-04-18 10:51:10.000000 ratinabox-1.4.2/ratinabox.egg-info/top_level.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      930 2023-04-18 10:51:10.489117 ratinabox-1.4.2/setup.cfg
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.4.2/setup.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-18 10:51:10.488539 ratinabox-1.4.2/tests/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-04-12 13:21:00.000000 ratinabox-1.4.2/tests/test_advanced.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.4.2/tests/test_agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.4.2/tests/test_environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.4.2/tests/test_neurons.py
```

### Comparing `ratinabox-1.4.1/LICENSE` & `ratinabox-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/PKG-INFO` & `ratinabox-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.4.1
+Version: 1.4.2
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
@@ -57,15 +57,15 @@
 * **Fast**:         Simulating 1 minute of exploration in a 2D environment with 100 place cells (dt=10 ms) take just 2 seconds on a laptop (no GPU needed).
 * **Precise**:      No more prediscretised positions, tabular state spaces, or jerky movement policies. It's all continuous. 
 * **Easy**:         Sensible default parameters mean you can have realisitic simulation data to work with in ~10 lines of code.
 * **Visual**        Plot or animate trajectories, firing rate timeseries', spike rasters, receptive fields, heat maps, velocity histograms...using the plotting functions ([summarised here](./demos/list_of_plotting_fuctions.md)). 
 
 
 ## Get started 
-Many [demos](./demos/) are provided. Reading through the [example scripts](#example-scripts) (one simple and one extensive, duplicated at the bottom of the readme) these should be enough to get started. We also provide numerous interactive jupyter scripts as more in-depth case studies; for example one where `RatInABox` is used for [reinforcement learning](./demos/reinforcement_learning_example.ipynb), another for [neural decoding](./demos/decoding_position_example.ipynb) of position from firing rate. Jupyter scripts reproducing all figures in the [paper](./demos/paper_figures.ipynb) and [readme](./demos/readme_figures.ipynb) are also provided.
+Many [demos](./demos/) are provided. Reading through the [example scripts](#example-scripts) (one simple and one extensive, duplicated at the bottom of the readme) these should be enough to get started. We also provide numerous interactive jupyter scripts as more in-depth case studies; for example one where `RatInABox` is used for [reinforcement learning](./demos/reinforcement_learning_example.ipynb), another for [neural decoding](./demos/decoding_position_example.ipynb) of position from firing rate. Jupyter scripts reproducing all figures in the [paper](./demos/paper_figures.ipynb) and [readme](./demos/readme_figures.ipynb) are also provided. All [demos](./demos/) can be run on Google Colab [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](./demos/)
 
 ## Installing and Importing
 **Requirements** are minimal (`python3`, `numpy`, `scipy` and `matplotlib`, listed in `setup.cfg`) and will be installed automatically. 
 
 **Install** the latest, stable version using `pip` at the command line with
 ```console
 $ pip install ratinabox
```

### Comparing `ratinabox-1.4.1/README.md` & `ratinabox-1.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 * **Fast**:         Simulating 1 minute of exploration in a 2D environment with 100 place cells (dt=10 ms) take just 2 seconds on a laptop (no GPU needed).
 * **Precise**:      No more prediscretised positions, tabular state spaces, or jerky movement policies. It's all continuous. 
 * **Easy**:         Sensible default parameters mean you can have realisitic simulation data to work with in ~10 lines of code.
 * **Visual**        Plot or animate trajectories, firing rate timeseries', spike rasters, receptive fields, heat maps, velocity histograms...using the plotting functions ([summarised here](./demos/list_of_plotting_fuctions.md)). 
 
 
 ## Get started 
-Many [demos](./demos/) are provided. Reading through the [example scripts](#example-scripts) (one simple and one extensive, duplicated at the bottom of the readme) these should be enough to get started. We also provide numerous interactive jupyter scripts as more in-depth case studies; for example one where `RatInABox` is used for [reinforcement learning](./demos/reinforcement_learning_example.ipynb), another for [neural decoding](./demos/decoding_position_example.ipynb) of position from firing rate. Jupyter scripts reproducing all figures in the [paper](./demos/paper_figures.ipynb) and [readme](./demos/readme_figures.ipynb) are also provided.
+Many [demos](./demos/) are provided. Reading through the [example scripts](#example-scripts) (one simple and one extensive, duplicated at the bottom of the readme) these should be enough to get started. We also provide numerous interactive jupyter scripts as more in-depth case studies; for example one where `RatInABox` is used for [reinforcement learning](./demos/reinforcement_learning_example.ipynb), another for [neural decoding](./demos/decoding_position_example.ipynb) of position from firing rate. Jupyter scripts reproducing all figures in the [paper](./demos/paper_figures.ipynb) and [readme](./demos/readme_figures.ipynb) are also provided. All [demos](./demos/) can be run on Google Colab [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](./demos/)
 
 ## Installing and Importing
 **Requirements** are minimal (`python3`, `numpy`, `scipy` and `matplotlib`, listed in `setup.cfg`) and will be installed automatically. 
 
 **Install** the latest, stable version using `pip` at the command line with
 ```console
 $ pip install ratinabox
```

### Comparing `ratinabox-1.4.1/ratinabox/Agent.py` & `ratinabox-1.4.2/ratinabox/Agent.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/ratinabox/Environment.py` & `ratinabox-1.4.2/ratinabox/Environment.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/ratinabox/Neurons.py` & `ratinabox-1.4.2/ratinabox/Neurons.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,14 +142,15 @@
         t_end=None,
         chosen_neurons="all",
         spikes=False,
         imshow=False,
         fig=None,
         ax=None,
         xlim=None,
+        color=None,
         background_color=None,
         autosave=None,
         **kwargs,
     ):
         """Plots a timeseries of the firing rate of the neurons between t_start and t_end
 
         Args:
@@ -158,14 +159,15 @@
             • chosen_neurons: Which neurons to plot. string "10" or 10 will plot ten of them, "all" will plot all of them, "12rand" will plot 12 random ones. A list like [1,4,5] will plot cells indexed 1, 4 and 5. Defaults to "all".
             chosen_neurons (str, optional): Which neurons to plot. string "10" will plot 10 of them, "all" will plot all of them, a list like [1,4,5] will plot cells indexed 1, 4 and 5. Defaults to "10".
             • spikes (bool, optional): If True, scatters exact spike times underneath each curve of firing rate. Defaults to True.
             the below params I just added for help with animations
             • imshow - if True will not dispaly as mountain plot but as an image (plt.imshow)
             • fig, ax: the figure, axis to plot on (can be None)
             xlim: fix xlim of plot irrespective of how much time you're plotting
+            • color: color of the line, if None, defaults to cell class default (probalby "C1")
             • background_color: color of the background if not matplotlib default (probably white)
             • autosave: if True, will try to save the figure to the figure directory `ratinabox.figure_directory`. Defaults to None in which case looks for global constant ratinabox.autosave_plots
             • kwargs sent to mountain plot function, you can ignore these
 
         Returns:
             fig, ax
         """
@@ -188,21 +190,22 @@
             kwargs["shift"] = max(
                 1.5, min(4, 40 / n_neurons_to_plot)
             )  # scaled to make plots look nice and be ~constant size
             kwargs["shift"] = 2
             kwargs["overlap"] = 2.2
         spike_data = spike_data[startid:endid, chosen_neurons]
         rate_timeseries = rate_timeseries[:, chosen_neurons]
-
+        if color is None:
+            color = self.color
         if imshow == False:
             firingrates = rate_timeseries.T
             fig, ax = utils.mountain_plot(
                 X=t / 60,
                 NbyX=firingrates,
-                color=self.color,
+                color=color,
                 xlabel="Time / min",
                 ylabel="Neurons",
                 xlim=None,
                 fig=fig,
                 ax=ax,
                 **kwargs,
             )
@@ -215,17 +218,23 @@
                         time_when_spiked,
                         h,
                         color=(self.color or "C1"),
                         alpha=0.5,
                         s=5,
                         linewidth=0,
                     )
-            ax.set_xlim(left=t_start / 60, right=t_end / 60)
-            ax.set_xticks([t_start / 60, t_end / 60])
-            ax.set_xticklabels([round(t_start / 60, 2), round(t_end / 60, 2)])
+
+            xmin = min(t_start / 60, ax.get_xlim()[0])
+            xmax = max(t_end / 60, ax.get_xlim()[1])
+            ax.set_xlim(
+                left=xmin,
+                right=xmax,
+            )
+            ax.set_xticks([xmin, xmax])
+            ax.set_xticklabels([round(xmin, 2), round(xmax, 2)])
             if xlim is not None:
                 ax.set_xlim(right=xlim / 60)
                 ax.set_xticks([round(t_start / 60, 2), round(xlim / 60, 2)])
                 ax.set_xticklabels([round(t_start / 60, 2), round(xlim / 60, 2)])
 
             if background_color is not None:
                 ax.set_facecolor(background_color)
@@ -1010,19 +1019,19 @@
         """Here we implement the same type if boundary vector cells as de Cothi et al. (2020), who follow Barry & Burgess, (2007). See equations there.
 
         The way we do this is a little complex. We will describe how it works from a single position (but remember this can be called in a vectorised manner from an array of positons in parallel)
             1. An array of normalised "test vectors" span, in all directions at small increments, from the current position
             2. These define an array of line segments stretching from [pos, pos+test vector]
             3. Where these line segments collide with all walls in the environment is established, this uses the function "utils.vector_intercepts()"
             4. This pays attention to only consider the first (closest) wall forawrd along a line segment. Walls behind other walls are "shaded" by closer walls. Its a little complex to do this and requires the function "boundary_vector_preference_function()"
-            5. Now that, for every test direction, the closest wall is established it is simple a process of finding the response of the neuron to that wall at that angle (multiple of two gaussians, see de Cothi (2020)) and then summing over all the test angles.
+            5. Now that, for every test direction, the closest wall is established it is simple a process of finding the response of the neuron to that wall segment at that angle (multiple of two gaussians, see de Cothi (2020)) and then summing over all wall segments for all test angles.
 
         We also apply a check in the middle to utils.rotate the reference frame into that of the head direction of the agent iff self.reference_frame='egocentric'.
 
-        By default position is taken from the Agent and used to calculate firing rates. This can also by passed directly (evaluate_at=None, pos=pass_array_of_positions) or ou can use all the positions in the environment (evaluate_at="all").
+        By default position is taken from the Agent and used to calculate firing rates. This can also by passed directly (evaluate_at=None, pos=pass_array_of_positions) or you can use all the positions in the environment (evaluate_at="all").
         """
         if evaluate_at == "agent":
             pos = self.Agent.pos
         elif evaluate_at == "all":
             pos = self.Agent.Environment.flattened_discrete_coords
         else:
             pos = kwargs["pos"]
```

### Comparing `ratinabox-1.4.1/ratinabox/README.md` & `ratinabox-1.4.2/ratinabox/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/ratinabox/__init__.py` & `ratinabox-1.4.2/ratinabox/__init__.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/ratinabox/contribs/FieldOfViewNeurons.py` & `ratinabox-1.4.2/ratinabox/contribs/FieldOfViewNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/ratinabox/contribs/PhasePrecessingPlaceCells.py` & `ratinabox-1.4.2/ratinabox/contribs/PhasePrecessingPlaceCells.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/ratinabox/contribs/PlaneWaveNeurons.py` & `ratinabox-1.4.2/ratinabox/contribs/PlaneWaveNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/ratinabox/contribs/README.md` & `ratinabox-1.4.2/ratinabox/contribs/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/ratinabox/contribs/STDPFeedForwardLayer.py` & `ratinabox-1.4.2/ratinabox/contribs/STDPFeedForwardLayer.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/ratinabox/contribs/ThetaSequenceAgent.py` & `ratinabox-1.4.2/ratinabox/contribs/ThetaSequenceAgent.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/ratinabox/contribs/ValueNeuron.py` & `ratinabox-1.4.2/ratinabox/contribs/ValueNeuron.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/ratinabox/data/README.md` & `ratinabox-1.4.2/ratinabox/data/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/ratinabox/data/rat.png` & `ratinabox-1.4.2/ratinabox/data/rat.png`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/ratinabox/data/sargolini.npz` & `ratinabox-1.4.2/ratinabox/data/sargolini.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/ratinabox/data/tanni.npz` & `ratinabox-1.4.2/ratinabox/data/tanni.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/ratinabox/utils.py` & `ratinabox-1.4.2/ratinabox/utils.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/ratinabox.egg-info/PKG-INFO` & `ratinabox-1.4.2/ratinabox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.4.1
+Version: 1.4.2
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
@@ -57,15 +57,15 @@
 * **Fast**:         Simulating 1 minute of exploration in a 2D environment with 100 place cells (dt=10 ms) take just 2 seconds on a laptop (no GPU needed).
 * **Precise**:      No more prediscretised positions, tabular state spaces, or jerky movement policies. It's all continuous. 
 * **Easy**:         Sensible default parameters mean you can have realisitic simulation data to work with in ~10 lines of code.
 * **Visual**        Plot or animate trajectories, firing rate timeseries', spike rasters, receptive fields, heat maps, velocity histograms...using the plotting functions ([summarised here](./demos/list_of_plotting_fuctions.md)). 
 
 
 ## Get started 
-Many [demos](./demos/) are provided. Reading through the [example scripts](#example-scripts) (one simple and one extensive, duplicated at the bottom of the readme) these should be enough to get started. We also provide numerous interactive jupyter scripts as more in-depth case studies; for example one where `RatInABox` is used for [reinforcement learning](./demos/reinforcement_learning_example.ipynb), another for [neural decoding](./demos/decoding_position_example.ipynb) of position from firing rate. Jupyter scripts reproducing all figures in the [paper](./demos/paper_figures.ipynb) and [readme](./demos/readme_figures.ipynb) are also provided.
+Many [demos](./demos/) are provided. Reading through the [example scripts](#example-scripts) (one simple and one extensive, duplicated at the bottom of the readme) these should be enough to get started. We also provide numerous interactive jupyter scripts as more in-depth case studies; for example one where `RatInABox` is used for [reinforcement learning](./demos/reinforcement_learning_example.ipynb), another for [neural decoding](./demos/decoding_position_example.ipynb) of position from firing rate. Jupyter scripts reproducing all figures in the [paper](./demos/paper_figures.ipynb) and [readme](./demos/readme_figures.ipynb) are also provided. All [demos](./demos/) can be run on Google Colab [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](./demos/)
 
 ## Installing and Importing
 **Requirements** are minimal (`python3`, `numpy`, `scipy` and `matplotlib`, listed in `setup.cfg`) and will be installed automatically. 
 
 **Install** the latest, stable version using `pip` at the command line with
 ```console
 $ pip install ratinabox
```

### Comparing `ratinabox-1.4.1/ratinabox.egg-info/SOURCES.txt` & `ratinabox-1.4.2/ratinabox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ratinabox-1.4.1/setup.cfg` & `ratinabox-1.4.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ratinabox
-version = 1.4.1
+version = 1.4.2
 author = Tom George
 author_email = tomgeorge1@btinternet.com
 project_urls = 
 	Documentation = https://github.com/TomGeorge1234/RatInABox
 	Source = https://github.com/TomGeorge1234/RatInABox
 	Tracker = https://github.com/TomGeorge1234/RatInABox/issues
 description = RatInABox: A package for simulating motion and ephys data in continuous environments
```

### Comparing `ratinabox-1.4.1/tests/test_advanced.py` & `ratinabox-1.4.2/tests/test_advanced.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # TO DO: write more detailed tests 
-# For now, test_advanced will simply try to run versions of the "simple", "extensive" and "decoding_position" demo scripts. Assuming no error is raised the test has passed. It will also test whether exteranl data (sargolini) can be imported to test data availability. 
+# For now, test_advanced will simply try to run versions of the "simple", "extensive" and "decoding_position" demo scripts. Assuming no error is raised the test has passed. It will also test whether external data (Sargolini) can be imported to test data availability. 
 # This is an okay safety net for now but should be improved in future versions
 
 #this test requires scikitlearn 
 
 import pytest
 import numpy as np 
 import matplotlib.pyplot as plt
```

### Comparing `ratinabox-1.4.1/tests/test_environment.py` & `ratinabox-1.4.2/tests/test_environment.py`

 * *Files identical despite different names*

