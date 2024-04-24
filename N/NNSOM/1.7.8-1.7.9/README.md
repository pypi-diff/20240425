# Comparing `tmp/nnsom-1.7.8.tar.gz` & `tmp/nnsom-1.7.9.tar.gz`

## Comparing `nnsom-1.7.8.tar` & `nnsom-1.7.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 nnsom-1.7.8/src/NNSOM/__init__.py
--rw-r--r--   0        0        0    77601 2020-02-02 00:00:00.000000 nnsom-1.7.8/src/NNSOM/plots.py
--rw-r--r--   0        0        0    19217 2020-02-02 00:00:00.000000 nnsom-1.7.8/src/NNSOM/som.py
--rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 nnsom-1.7.8/src/NNSOM/som_gpu.py
--rw-r--r--   0        0        0    20937 2020-02-02 00:00:00.000000 nnsom-1.7.8/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16111 2020-02-02 00:00:00.000000 nnsom-1.7.8/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.7.8/LICENSE
--rw-r--r--   0        0        0     8461 2020-02-02 00:00:00.000000 nnsom-1.7.8/README.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 nnsom-1.7.8/pyproject.toml
--rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 nnsom-1.7.8/PKG-INFO
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 nnsom-1.7.9/src/NNSOM/__init__.py
+-rw-r--r--   0        0        0    96075 2020-02-02 00:00:00.000000 nnsom-1.7.9/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    19217 2020-02-02 00:00:00.000000 nnsom-1.7.9/src/NNSOM/som.py
+-rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 nnsom-1.7.9/src/NNSOM/som_gpu.py
+-rw-r--r--   0        0        0    20937 2020-02-02 00:00:00.000000 nnsom-1.7.9/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16111 2020-02-02 00:00:00.000000 nnsom-1.7.9/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.7.9/LICENSE
+-rw-r--r--   0        0        0     8461 2020-02-02 00:00:00.000000 nnsom-1.7.9/README.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 nnsom-1.7.9/pyproject.toml
+-rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 nnsom-1.7.9/PKG-INFO
```

### Comparing `nnsom-1.7.8/src/NNSOM/plots.py` & `nnsom-1.7.9/src/NNSOM/plots.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,82 +15,74 @@
 from matplotlib.widgets import Button
 from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 import matplotlib.colors as mcolors
 
 
 class SOMPlots(base_class):
     """
-    SOMPlots extends the SOM class by adding visualization capabilities to
-    the Self-Organizing Map (SOM). It allows for the graphical representation
-    of the SOM's structure, the distribution of input data across its neurons,
-    and various other analytical visualizations that aid in the interpretation
-    of the SOM's behavior and characteristics.
+    A subclass of either SOM or SOMGpu (based on the availability of CuPy), designed to provide visualization
+    and interactive plotting capabilities for Self-Organizing Maps (SOMs). This class is intended to enrich the analysis
+    of SOMs by offering a variety of advanced visualization techniques to explore the trained SOM topology,
+    distribution of data points, and various statistics derived from the SOM's learning process.
 
     Attributes:
-        dimensions (tuple): The dimensions of the SOM grid.
+        dimensions: A Gird of the SOM topology.
 
     Methods:
-        plt_top():
-            Plots the topology of the SOM using hexagonal units.
-        plt_top_num():
-            Plots the topology of the SOM with numbered neurons.
-        hit_hist(x, textFlag):
-            Plots a hit histogram showing how many data points are mapped to each neuron.
-        gray_hist(x, perc):
-            Plots a histogram with neurons colored in shades of gray based on a given percentage value.
-        color_hist(x, avg):
-            Plots a color-coded histogram based on the average values provided for each neuron.
-        cmplx_hit_hist(x, perc_gb, clust, ind_missClass, ind21, ind12):
-            Plots a complex hit histogram showing the distribution of data and misclassifications.
-        plt_nc():
-            Plots the neighborhood connections between the SOM neurons.
-        neuron_dist_plot():
-            Plots the distances between neurons to visualize the SOM's topology.
-        simple_grid(avg, sizes):
-            Plots a simple hexagonal grid with varying colors and sizes based on provided data.
-        setup_axes():
-            Sets up the axes for plotting individual neuron statistics.
-        plt_dist(dist):
-            Plots distributions of values across the SOM neurons.
-        plt_wgts():
-            Plots the weights of the SOM neurons as line graphs.
-        plt_pie(title, perc, *argv):
-            Plots pie charts for each neuron to show data distribution in categories.
-        plt_histogram(som, data):
-            Plots histograms for each neuron to show the distribution of data.
-        plt_boxplot(data):
-            Plots boxplots for each neuron to show the distribution of data.
-        plt_dispersion_fan_plot(data):
-            Plots dispersion or fan plots for each neuron.
-        plt_violin_plot(som, data):
-            Plots violin plots for each neuron to show the distribution of data.
-        plt_scatter(x, indices, clust, reg_line=True):
-            Plots scatter graphs for each neuron to show the distribution of two variables.
-        multiplot(plot_type, *args):
-            Facilitates plotting of multiple types of graphs based on the plot_type argument.
+        The class includes methods for plotting the topology of the SOM, generating hit histograms,
+        displaying cluster information, and more. These methods support interactive features through
+        mouse clicks, allowing users to engage with the visualizations dynamically. Each method
+        can also handle additional parameters for customization and handles various plotting styles
+        like hexagonal units, numbered neurons, color gradients, and complex cluster histograms.
+        The class also provides a generic plot method to handle different types of SOM visualizations
+        and an event handling method to manage user interactions during the plotting sessions.
+
+    This class supports interactivity and offers multiple visualization methods to deeply understand
+    and analyze the behaviors and results of SOMs. It's especially useful for gaining insights into
+    the topology, data distribution, and classification performance of SOMs.
     """
+
     def __init__(self, dimensions):
+        """
+        Initializes the SOMPlots class with specified dimensions for the SOM grid. This constructor
+        sets up the underlying SOM or SOMGpu infrastructure, depending on the availability of CuPy.
+
+        Parameters
+        ----------
+        dimensions : array-like, tuple, or int
+            A tuple specifying the dimensions (rows, columns) of the SOM grid.
+        """
         super().__init__(dimensions)
 
     def plt_top(self, mouse_click=False, connect_pick_event=True, **kwargs):
-        """ Plots the topology of the SOM using hexagonal units.
+        """
+        Plots the topology of the SOM using hexagonal units. This method visualizes the position and the
+        boundaries of each neuron within the grid, allowing for interaction if enabled.
 
-        Args:
-            mouse_click: bool
-                If true, the interactive plot and sub-clustering functionalities to be activated
-            connect_pick_event: bool
-                If true, the pick event is connected to the plot
-            kwarg: dict
-                Additional arguments to be passed to the onpick function
-                Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
+        Parameters
+        ----------
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing interactive functionality such as
+            querying or modifying neuron data, by default False.
+        connect_pick_event : bool, optional
+            If True, connects a pick event that triggers when a neuron (hexagon) is clicked, by default True.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler `onpick` when an interactive
+            element is clicked. Common parameters could include data specific to the plot or visualization settings.
 
-        Returns:
-            fig, ax, pathces
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        patches : list
+            A list of matplotlib.patches.Patch objects representing the hexagonal units of the SOM.
         """
+
         w = self.w
         pos = self.pos
         numNeurons = self.numNeurons
 
         shapex, shapey = get_hexagon_shape()
 
         fig, ax = plt.subplots(frameon=False)
@@ -119,28 +111,39 @@
 
         # Get rid of extra white space on sides
         plt.tight_layout()
 
         return fig, ax, patches
 
     def plt_top_num(self, mouse_click=False, connect_pick_event=True, **kwargs):
-        """ Plots the topology of the SOM with numbered neurons.
+        """
+        Plots the topology of the SOM with each neuron numbered. This method visualizes each neuron as a hexagon with a
+        number indicating its index, which is useful for identifying and referencing specific neurons during analysis.
 
-        Args:
-            mouse_click: bool
-                If true, the interactive plot and sub-clustering functionalities to be activated
-            connect_pick_event: bool
-                If true, the pick event is connected to the plot
-            kwarg: dict
-                Additional arguments to be passed to the onpick function
-                Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
+        Parameters
+        ----------
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing for interaction such as detailed queries or
+            data manipulation associated with specific neurons, by default False.
+        connect_pick_event : bool, optional
+            If True, connects a pick event that triggers when a neuron is clicked, by default True.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler `onpick` when an interactive
+            element is clicked. Common parameters could include data specific to the plot or visualization settings.
 
-        Returns:
-            fig, ax, pathces, text
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        patches : list
+            A list of matplotlib.patches.Patch objects representing the hexagonal units of the SOM.
+        text : list
+            A list of matplotlib.text.Text objects displaying the neuron indices.
         """
         w = self.w
         pos = self.pos
         numNeurons = self.numNeurons
 
         shapex, shapey = get_hexagon_shape()
 
@@ -179,35 +182,44 @@
 
         # Get rid of extra white space on sides
         plt.tight_layout()
 
         return fig, ax, patches, text
 
     def hit_hist(self, x, textFlag=True, mouse_click=False, connect_pick_event=True, **kwargs):
-        """ Generate Hit Histogram
+        """
+        Generates a hit histogram for the SOM, which displays the frequency of data points assigned to each neuron.
+        Each neuron is represented as a hexagon, and the size of each hexagon is proportional to the number of hits.
+        Optionally, the actual number of hits can be displayed within each hexagon.
 
         Parameters
         ----------
-        x: array-like
-            The input data to be clustered
-        textFlag: bool
-            If true, the number of members of each cluster is printed on the cluster.
-        mouse_click: bool
-            If true, the interactive plot and sub-clustering functionalities to be activated
-        connect_pick_event
-            If true, the pick event is connected to the plot
-        kwargs: dict
-            Additional arguments to be passed to the on_pick function
-            Possible keys includes:
-            'data', 'labels', 'clust', 'target', 'num1', 'num2',
-            'cat', and 'topn'
+        x : array-like
+            The input data to be visualized in the histogram.
+        textFlag : bool, optional
+            If True, displays the count of hits within each hexagon, by default True.
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing for interactive functionality such as
+            querying or modifying neuron data, by default False.
+        connect_pick_event : bool, optional
+            If True, connects a pick event that triggers when a neuron is clicked, by default True.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler `onpick` when an interactive
+            element is clicked. Common parameters could include data specific to the plot or visualization settings.
 
         Returns
         -------
-            fig, ax, patches, text
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        patches : list
+            A list of matplotlib.patches.Patch objects representing the inner hexagons colored based on hit counts.
+        text : list, optional
+            A list of matplotlib.text.Text objects displaying the hit counts, included if textFlag is True.
         """
 
         pos = self.pos
         numNeurons = self.numNeurons
 
         # Determine the shape of the hexagon to represent each cluster
         shapex, shapey = get_hexagon_shape()
@@ -284,18 +296,39 @@
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, patches, text
 
     def gray_hist(self, x, perc, mouse_click=False, **kwargs):
-        # Make another hit histogram figure, and change the colors of the hexagons
-        # to indicate the perc of pdb (or gb) ligands in each cluster. Lighter color
-        # means more PDB ligands, darker color means more well-docked bad binders.
+        """
+        Generates a grayscale histogram for the SOM, where the shade of each hexagon represents the corresponding value from the provided percentage array.
 
+        Parameters
+        ----------
+        x : array-like
+            The input data to be visualized in the histogram.
+        perc : array-like
+            An array containing the percentage values to be represented by the grayscale shades, where higher values correspond to darker shades.
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing for interactive functionality such as querying or modifying neuron data, by default False.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler onpick when an interactive element is clicked. Common parameters could include data specific to the plot or visualization settings.
+
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        patches : list
+            A list of matplotlib.patches.Patch objects representing the inner hexagons colored based on the grayscale values.
+        text : list, optional
+            A list of matplotlib.text.Text objects displaying the hit counts, included if textFlag is True in the underlying `hit_hist` method.
+        """
         numNeurons = self.numNeurons
         dmax = np.amax(np.abs(perc))    # Find the maximum value of perc across all clusters
 
         fig, ax, patches, text = self.hit_hist(x, False, mouse_click, **kwargs)
 
         # Scale the gray scale to the perc value
         for neuron in range(numNeurons):
@@ -306,18 +339,41 @@
 
         # Get rid of extra white space on sides
         plt.tight_layout()
 
         return fig, ax, patches, text
 
     def color_hist(self, x, avg, mouse_click=False, **kwargs):
-        # Plot an SOM figure where the size of the hexagons is related to
-        # the number of elements in the clusters, and the color of the
-        # inner hexagon is coded to the variable avg, which could be the
-        # average number of a certain type of bond in the cluster
+        """
+        Generates a colored histogram for the SOM, where the color of each hexagon represents the corresponding value from the provided average array.
+
+        Parameters
+        ----------
+        x : array-like
+            The input data to be visualized in the histogram.
+        avg : array-like
+            An array containing the average values to be represented by the color map, where higher values correspond to warmer colors (e.g., red) and lower values correspond to cooler colors (e.g., blue).
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing for interactive functionality such as querying or modifying neuron data, by default False.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler onpick when an interactive element is clicked. Common parameters could include data specific to the plot or visualization settings.
+
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        patches : list
+            A list of matplotlib.patches.Patch objects representing the inner hexagons colored based on the average values.
+        text : list, optional
+            A list of matplotlib.text.Text objects displaying the hit counts, included if textFlag is True in the underlying `hit_hist` method.
+        cbar : matplotlib.colorbar.Colorbar
+            The Colorbar object attached to the plot, representing the color mapping.
+        """
 
         # Find the maximum value of avg across all clusters
         dmax = np.amax(np.abs(avg))
         numNeurons = self.numNeurons
 
         fig, ax, patches, text = self.hit_hist(x, False, mouse_click, **kwargs)
 
@@ -359,30 +415,46 @@
 
         # Get rid of extra white space on sides
         fig.tight_layout()
 
         return fig, ax, patches, text, cbar
 
     def cmplx_hit_hist(self, x, clust, perc, ind_missClass, ind21, ind12, mouse_click=False, **kwargs):
-        """ Generates a complex hit histogram.
-        It indicates what the majority class in each cluster is, and how many specific class occur in each cluster.
+        """
+        Generates a complex hit histogram for the SOM, incorporating information about cluster quality, misclassifications, and false positives/negatives.
 
-        Args:
-            x: array-like
-                The input data to be clustered
-            clust: list
-                List of indices of inputs that belong in each cluster
-            perc: array-like
-                Percent of the specific class in each cluster
-            ind_missClass: array-like
-                Indices of consistently misclassified inputs
-            ind21: array-like
-                Indices of false positive cases
-            ind12: array-like
-                Indices of false negative cases
+        Parameters
+        ----------
+        x : array-like
+            The input data to be visualized in the histogram.
+        clust : list or array-like
+            A list or array containing the cluster assignments for each data point.
+        perc : array-like
+            An array containing the percentage values for each cluster, representing the proportion of good binders.
+        ind_missClass : array-like
+            An array containing the indices of misclassified data points.
+        ind21 : array-like
+            An array containing the indices of false positive data points (classified as good binders but are actually bad binders).
+        ind12 : array-like
+            An array containing the indices of false negative data points (classified as bad binders but are actually good binders).
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing for interactive functionality such as querying or modifying neuron data, by default False.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler onpick when an interactive element is clicked. Common parameters could include data specific to the plot or visualization settings.
+
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        patches : list
+            A list of matplotlib.patches.Patch objects representing the inner hexagons colored and styled based on cluster quality and misclassifications.
+        text : list
+            A list of matplotlib.text.Text objects displaying the hit counts within each hexagon.
         """
 
         numNeurons = self.numNeurons
 
         if mouse_click:
             kwargs['clust'] = clust
 
@@ -415,38 +487,49 @@
 
         # Get rid of extra white space on sides
         plt.tight_layout()
 
         return fig, ax, patches, text
 
     def custom_cmplx_hit_hist(self, x, face_labels, edge_labels, edge_width, mouse_click=False, **kwargs):
-        """ Generate cmplex hit hist
-        Users can specify the face color, edge width and edge color for each neuron.
+        """
+        Generates a custom complex hit histogram for the SOM, allowing for flexible customization of the hexagon face colors, edge colors, and edge widths.
 
-        x: array-like or sequence of vectors
-            The input data to be clustered
-        face_labels: array-like
-            class labels to determine the face color of the hexagons
-        edge_labels: array-like
-            class labels to determine the edge color of the hexagons
-        edge_width: array-like
-            A list of edge_width standerdised between (1 - 20).
-            You can call get_edge_width to get the standardised edge width in the utils function.
-            len(edge_width) must be equal to the number of neurons
-        mouse_click: bool
-            If true, the interactive plot and sub-clustering functionalities to be activated
-        kwargs: dict
-            Additional arguments to be passed to the onpick function
-            Possible keys include:
-            'data', 'clust', 'target', 'num1', 'num2',
-            'cat', and 'topn'
+        Parameters
+        ----------
+        x : array-like
+            The input data to be visualized in the histogram.
+        face_labels : array-like
+            An array containing the labels or values to be represented by the face colors of the hexagons.
+        edge_labels : array-like
+            An array containing the labels or values to be represented by the edge colors of the hexagons.
+        edge_width : array-like
+            An array containing the values for the edge widths of the hexagons.
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing for interactive functionality such as querying or modifying neuron data, by default False.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler onpick when an interactive element is clicked. Common parameters could include data specific to the plot or visualization settings.
 
-        Returns:
-            fig, ax, patches, text
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        patches : list
+            A list of matplotlib.patches.Patch objects representing the inner hexagons colored and styled based on the provided face labels, edge labels, and edge widths.
+        text : list
+            A list of matplotlib.text.Text objects displaying the hit counts within each hexagon.
+
+        Raises
+        ------
+        ValueError
+            If the input data or label arrays have incorrect dimensions or lengths.
         """
+
         numNeurons = self.numNeurons
 
         x = np.asarray(x, np.float32)
         face_labels = np.asarray(face_labels, np.float32)
         edge_labels = np.asarray(edge_labels, np.float32)
         edge_width = np.asarray(edge_width, np.float32)
 
@@ -491,29 +574,34 @@
 
         # Get rid of extra white space on sides
         plt.tight_layout()
 
         return fig, ax, patches, text
 
     def plt_nc(self, mouse_click=False, connect_pick_event=True, **kwargs):
-        """ Generates neighborhood connection map.
-        The gray hexagons represent cluster centers.
+        """
+        Generates a Neighborhood Connection Map for the SOM, displaying the connections between neighboring neurons.
 
-        Args:
-            mouse_click: bool
-                If true, the interactive plot and sub-clustering functionalities to be activated
-            connect_pick_event: bool
-                If true, the pick event is connected to the plot
-            kwarg: dict
-                Additional arguments to be passed to the onpick function
-                Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
+        Parameters
+        ----------
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing for interactive functionality such as querying or modifying neuron data, by default False.
+        connect_pick_event : bool, optional
+            If True, connects a pick event that triggers when a neuron is clicked, by default True.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler onpick when an interactive element is clicked. Common parameters could include data specific to the plot or visualization settings.
 
-        Returns:
-            fig, ax, pathces
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        patches : list
+            A list of matplotlib.patches.Patch objects representing the edges between connected neurons.
         """
         # Neighborhood Connection Map. The gray hexagons represent cluster centers.
         pos = self.pos
         numNeurons = self.numNeurons
 
         # Determine the hexagon shape
         shapex, shapey = get_hexagon_shape()
@@ -566,30 +654,34 @@
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, patches
 
     def neuron_dist_plot(self, mouse_click=False, connect_pick_event=True, **kwargs):
-        """ Generates distance map.
-        The gray hexagons represent cluster centers.
-        The colors of the elongated hexagons between the cluster centers represent the distance between the centers.
-        The darker the color the larget the distance.
+        """
+        Generates a neuron distance plot that visualizes the distances between neighboring neurons in the SOM grid.
 
-        Args:
-            mouse_click: bool
-                If true, the interactive plot and sub-clustering functionalities to be activated
-            connect_pick_event: bool
-                If true, the pick event is connected to the plot
-            kwarg: dict
-                Additional arguments to be passed to the onpick function
-                Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
-        Returns:
-            fig, ax, pathces, text
+        Parameters
+        ----------
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing for interactive functionality such as querying or modifying neuron data, by default False.
+        connect_pick_event : bool, optional
+            If True, connects a pick event that triggers when a neuron is clicked, by default True.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler onpick when an interactive element is clicked. Common parameters could include data specific to the plot or visualization settings.
+
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        patches : list
+            A list of matplotlib.patches.Patch objects representing the edges between connected neurons, colored based on the distance between their respective neuron weights.
         """
 
         pos = self.pos
         numNeurons = self.numNeurons
 
         # Determine the shape of the hexagon to represent each cluster
         symmetry = 6
@@ -676,34 +768,40 @@
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, patches
 
     def simple_grid(self, avg, sizes, mouse_click=False, connect_pick_event=True, **kwargs):
-        """ Basic hexagon grid plot
-        Colors are selected from avg array.
-        Sizes of inner hexagons are selected rom sizes array.
+        """
+        Generates a simple grid plot that visualizes the SOM neurons as hexagons with varying sizes and colors.
 
-        Args:
-            avg: array-like
-                Average values for each neuron
-            sizes: array-like
-                Sizes of inner hexagons
-            mouse_click: bool
-                If true, the interactive plot and sub-clustering functionalities to be activated
-            connect_pick_event: bool
-                If true, the pick event is connected to the plot
-            kwarg: dict
-                Additional arguments to be passed to the onpick function
-                Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
+        Parameters
+        ----------
+        avg : array-like
+            An array containing the average values to be represented by the color map, where higher values correspond to warmer colors (e.g., red) and lower values correspond to cooler colors (e.g., blue).
+        sizes : array-like
+            An array containing the sizes to be used for the inner hexagons within each neuron, where larger values result in larger hexagons.
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing for interactive functionality such as querying or modifying neuron data, by default False.
+        connect_pick_event : bool, optional
+            If True, connects a pick event that triggers when a neuron is clicked, by default True.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler onpick when an interactive element is clicked. Common parameters could include data specific to the plot or visualization settings.
 
-        Returns:
-            fig, ax, pathces, cbar
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        patches : list
+            A list of matplotlib.patches.Patch objects representing the inner hexagons colored based on the average values and sized based on the provided sizes.
+        cbar : matplotlib.colorbar.Colorbar
+            The Colorbar object attached to the plot, representing the color mapping.
         """
 
         w = self.w
         pos = self.pos
         numNeurons = self.numNeurons
 
         # Determine the shape of the hexagon to represent each cluster
@@ -882,32 +980,38 @@
                                         bbox_transform=ax.transAxes, borderpad=0)
             h_axes[neuron].set(xticks=[], yticks=[])
             h_axes[neuron].set_frame_on(False)
 
         return fig, ax, h_axes, hexagons, hexagon_to_neuron
 
     def plt_stem(self, x, y, mouse_click=False, connect_pick_event=True, **kwargs):
-        """ Generate stem plot for each neuron.
+        """
+        Generates a stem plot visualization for the SOM, displaying the input data and neuron responses.
 
-        Args:
-            x: array-like
-                The x-axis values (align)
-            y: array-like or sequence of vectors
-                The y-axis values (height)
-            mouse_click: bool
-                If true, the interactive plot and sub-clustering functionalities to be activated
-            connect_pick_event: bool
-                If true, the pick event is connected to the plot
-            kwarg: dict
-                Additional arguments to be passed to the onpick function
-                Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
+        Parameters
+        ----------
+        x : array-like
+            The input data or independent variable for the stem plot.
+        y : array-like
+            The neuron responses or dependent variable for the stem plot, where each row corresponds to a neuron.
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing for interactive functionality such as querying or modifying neuron data, by default False.
+        connect_pick_event : bool, optional
+            If True, connects a pick event that triggers when a neuron is clicked, by default True.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler onpick when an interactive element is clicked. Common parameters could include data specific to the plot or visualization settings.
 
-        Returns:
-            fig, ax, h_axes
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        h_axes : list
+            A list of matplotlib.axes.Axes objects, each containing a stem plot for a single neuron.
         """
 
         numNeurons = self.numNeurons
 
         # Setup figure, axes, and sub-axes
         fig, ax, h_axes, hexagons, hexagon_to_neuron = self.setup_axes()
 
@@ -921,28 +1025,34 @@
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, h_axes
 
     def plt_wgts(self, mouse_click=False, connect_pick_event=True, **kwargs):
-        """ Generate line plot for each neuron.
+        """
+        Generates a line plot visualization for the SOM weights, displaying the weight vectors for each neuron.
 
-        Args:
-            mouse_click: bool
-                If true, the interactive plot and sub-clustering functionalities to be activated
-            connect_pick_event: bool
-                If true, the pick event is connected to the plot
-            kwarg: dict
-                Additional arguments to be passed to the onpick function
-                Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
+        Parameters
+        ----------
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing for interactive functionality such as querying or modifying neuron data, by default False.
+        connect_pick_event : bool, optional
+            If True, connects a pick event that triggers when a neuron is clicked, by default True.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler onpick when an interactive element is clicked. Common parameters could include data specific to the plot or visualization settings.
 
-        Returns:
-            fig, ax, h_axes
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        h_axes : list
+            A list of matplotlib.axes.Axes objects, each containing a line plot for a single neuron's weight vector.
         """
 
         numNeurons = self.numNeurons
         w = self.w
 
         # Setup figure, main axes, and sub-axes
         fig, ax, h_axes, hexagons, hexagon_to_neuron = self.setup_axes()
@@ -956,34 +1066,45 @@
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, h_axes
 
     def plt_pie(self, x, s=None, mouse_click=False, connect_pick_event=True, **kwargs):
-        """ Generate pie plot for each neuron.
+        """
+        Generates a pie chart visualization for the SOM, displaying the composition of each neuron's data or cluster.
 
-        Args:
-            x: Array or sequence of vectors.
-                The wedge size
-            s: 1-D array-like, optional
-                Scale the size of the pie chart according to the percent of the specific class in that cell. (0-100)
-                (default: None)
-            mouse_click: bool
-                If true, the interactive plot and sub-clustering functionalities to be activated
-            connect_pick_event: bool
-                If true, the pick event is connected to the plot
-            kwarg: dict
-                Additional arguments to be passed to the onpick function
-                Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
+        Parameters
+        ----------
+        x : array-like
+            A 2D array or sequence of vectors, where each row represents the composition or category values for a single neuron.
+        s : array-like, optional
+            An array containing the percentage values to be used for scaling the pie chart sizes, by default None.
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing for interactive functionality such as querying or modifying neuron data, by default False.
+        connect_pick_event : bool, optional
+            If True, connects a pick event that triggers when a neuron is clicked, by default True.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler onpick when an interactive element is clicked. Common parameters could include data specific to the plot or visualization settings.
 
-        Returns:
-            fig, ax, h_axes
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        h_axes : list
+            A list of matplotlib.axes.Axes objects, each containing a pie chart for a single neuron's composition.
+
+        Raises
+        ------
+        ValueError
+            If the length of `x` or `s` (if provided) does not match the number of neurons, or if the percentage values in `s` are not between 0 and 100.
         """
+
         # Validate the length of x (array or sequence of vectors)
         if len(x) != self.numNeurons:
             raise ValueError("The length of x must be equal to the number of neurons.")
 
         # Validate perc values
         if s is not None:
             s = np.array(s)
@@ -1027,32 +1148,37 @@
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, h_axes
 
     def plt_histogram(self, x, mouse_click=False, connect_pick_event=True, **kwargs):
-        """ Generate histogram for each neuron.
+        """
+        Generates a histogram visualization for the SOM, displaying the data distribution within each neuron's cluster.
 
-        Args:
-            x: array-like
-                The input data to be plotted in histogram
-            mouse_click: bool
-                If true, the interactive plot and sub-clustering functionalities to be activated
-            connect_pick_event: bool
-                If true, the pick event is connected to the plot
-            kwarg: dict
-                Additional arguments to be passed to the onpick function
-                Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
+        Parameters
+        ----------
+        x : array-like
+            A 2D array or sequence of vectors, where each row represents the data points assigned to a single neuron.
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing for interactive functionality such as querying or modifying neuron data, by default False.
+        connect_pick_event : bool, optional
+            If True, connects a pick event that triggers when a neuron is clicked, by default True.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler onpick when an interactive element is clicked. Common parameters could include data specific to the plot or visualization settings.
 
-        Returns:
-            fig, ax, h_axes
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        h_axes : list
+            A list of matplotlib.axes.Axes objects, each containing a histogram for a single neuron's data distribution.
         """
-
         numNeurons = self.numNeurons
 
         # Setup figure, main axes, and sub-axes
         fig, ax, h_axes, hexagons, hexagon_to_neuron = self.setup_axes()
 
         # Draw histogram
         for neuron in range(numNeurons):
@@ -1078,30 +1204,36 @@
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, h_axes
 
     def plt_boxplot(self, x, mouse_click=False, connect_pick_event=True, **kwargs):
-        """ Generate box plot for each neuron.
+        """
+        Generates a boxplot visualization for the SOM, displaying the statistical summary of the data distribution within each neuron's cluster.
 
-        Args:
-            x: array-like
-                The input data to be plotted in box plot
-            mouse_click: bool
-                If true, the interactive plot and sub-clustering functionalities to be activated
-            connect_pick_event: bool
-                If true, the pick event is connected to the plot
-            kwarg: dict
-                Additional arguments to be passed to the onpick function
-                Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
+        Parameters
+        ----------
+        x : array-like
+            A 2D array or sequence of vectors, where each row represents the data points assigned to a single neuron.
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing for interactive functionality such as querying or modifying neuron data, by default False.
+        connect_pick_event : bool, optional
+            If True, connects a pick event that triggers when a neuron is clicked, by default True.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler onpick when an interactive element is clicked. Common parameters could include data specific to the plot or visualization settings.
 
-        Returns:
-            fig, ax, h_axes
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        h_axes : list
+            A list of matplotlib.axes.Axes objects, each containing a boxplot for a single neuron's data distribution.
         """
 
         numNeurons = self.numNeurons
 
         # Setup figure, main axes, and sub-axes
         fig, ax, h_axes, hexagons, hexagon_to_neuron = self.setup_axes()
 
@@ -1124,30 +1256,36 @@
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, h_axes
 
     def plt_violin_plot(self, x, mouse_click=False, connect_pick_event=True, **kwargs):
-        """ Generate violin plot for each neuron.
+        """
+        Generates a violin plot visualization for the SOM, displaying the distribution of data within each neuron's cluster.
 
-        Args:
-            x: array-like
-                The input data to be plotted in violin plot
-            mouse_click: bool
-                If true, the interactive plot and sub-clustering functionalities to be activated
-            connect_pick_event: bool
-                If true, the pick event is connected to the plot
-            kwarg: dict
-                Additional arguments to be passed to the onpick function
-                Possible keys include:
-                    'data', 'clust', 'target', 'num1', 'num2', 'cat', and 'topn'
+        Parameters
+        ----------
+        x : array-like
+            A 2D array or sequence of vectors, where each row represents the data points assigned to a single neuron.
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing for interactive functionality such as querying or modifying neuron data, by default False.
+        connect_pick_event : bool, optional
+            If True, connects a pick event that triggers when a neuron is clicked, by default True.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler onpick when an interactive element is clicked. Common parameters could include data specific to the plot or visualization settings.
 
-        Returns:
-            fig, ax, h_axes
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        h_axes : list
+            A list of matplotlib.axes.Axes objects, each containing a violin plot for a single neuron's data distribution.
         """
 
         numNeurons = self.numNeurons
 
         # Setup figure, main axes, and sub-axes
         fig, ax, h_axes, hexagons, hexagon_to_neuron = self.setup_axes()
 
@@ -1170,25 +1308,42 @@
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, h_axes
 
     def plt_scatter(self, x, y, reg_line=True, mouse_click=False, connect_pick_event=True, **kwargs):
-        """ Generate Scatter Plot for Each Neuron.
+        """
+        Generates a scatter plot visualization for the SOM, displaying the data points assigned to each neuron and an optional regression line.
 
-        Args:
-            x: input data
-            indices: array-like indices e.g. (0, 1) or [0, 1]
-            clust: list of indices of input data for each cluster
-            reg_line: Flag
+        Parameters
+        ----------
+        x : array-like
+            A 2D array or sequence of vectors, where each row represents the x-coordinate data points assigned to a single neuron.
+        y : array-like
+            A 2D array or sequence of vectors, where each row represents the y-coordinate data points assigned to a single neuron.
+        reg_line : bool, optional
+            If True, a regression line is plotted for each neuron's data, by default True.
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing for interactive functionality such as querying or modifying neuron data, by default False.
+        connect_pick_event : bool, optional
+            If True, connects a pick event that triggers when a neuron is clicked, by default True.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler onpick when an interactive element is clicked. Common parameters could include data specific to the plot or visualization settings.
 
-        Returns:
-            fig, ax, h_axes
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        h_axes : list
+            A list of matplotlib.axes.Axes objects, each containing a scatter plot for a single neuron's data.
         """
+
         pos = self.pos
         numNeurons = self.numNeurons
 
         # Setup figure, main axes, and sub-axes
         fig, ax, h_axes, hexagons, hexagon_to_neuron = self.setup_axes()
 
         # Determine the global minimum and maximum of x and y for the axes limits
@@ -1229,19 +1384,23 @@
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, h_axes
 
     def component_positions(self, x):
         """
-        Plots the SOM weight vectors, the Iris dataset input vectors, and connects neighboring neurons.
+        Visualizes the positions of the components in a Self-Organizing Map (SOM) along with the input vectors.
 
-        Parameters:
-        - som: A trained SOM instance with attributes 'w' for weight vectors and 'dimensions' for grid dimensions.
-        - X_scaled: The normalized Iris dataset input vectors.
+        This method plots the trained SOM weight vectors as gray dots and the input vectors as green dots on a 2D plot.
+        It also connects neighboring SOM neurons with red lines to represent the grid structure, illustrating the organization and clustering within the map.
+
+        Parameters
+        ----------
+        x : array-like
+            A 2D array or sequence of vectors, typically representing input data or test data that has been projected onto the SOM.
         """
 
         x = np.transpose(x)
 
         # Extract the trained weight vectors and the SOM grid dimensions
         weight_vectors = self.w
         grid_x, grid_y = self.dimensions
@@ -1277,14 +1436,25 @@
         plt.ylabel('Weight 2')
         plt.title('SOM Weight Positions')
         plt.legend()
         plt.grid(False)
         plt.show()
 
     def component_planes(self, X):
+        """
+        Visualizes the weight distribution across different features in a Self-Organizing Map (SOM) using a series of 2D plots.
+
+        This method creates a grid of subplots where each subplot represents the weight distribution for a specific feature of the input data. The weight of each neuron for the given feature is represented in the plot by the color of a hexagonal cell, with darker colors indicating higher weights. This visualization helps in understanding the importance and distribution of each feature across the map.
+
+        Parameters
+        ----------
+        X : array-like
+            A 2D array of input data where each row represents a feature and each column represents a sample.
+        """
+
         w = self.w
         pos = self.pos
         numNeurons = self.numNeurons
         z = np.sqrt(0.75)
         shapex = np.array([-1, 0, 1, 1, 0, -1]) * 0.5
         shapey = np.array([1, 2, 1, -1, -2, -1]) * (z / 3)
 
@@ -1313,15 +1483,41 @@
                     color = plt.cm.viridis(norm(feature_weights[j]))  # Choose colormap as viridis
                     inverted_color = tuple(
                         1 - np.array(color[:3]))  # Invert the color to make darker colors represent larger weights
                     ax.fill(pos[0, j] + shapex, pos[1, j] + shapey, facecolor=inverted_color, edgecolor=(0.8, 0.8, 0.8))
 
         plt.show()
 
-    def weight_as_image(self, rows= None, mouse_click=False, connect_pick_event=True, **kwargs):
+    def weight_as_image(self, rows=None, mouse_click=False, connect_pick_event=True, **kwargs):
+        """
+        Visualizes the weights of a Self-Organizing Map (SOM) as images within a hexagonal grid layout.
+
+        This method maps the weight vectors of each neuron onto a hexagonal cell and optionally enables interaction with each hexagon. The hexagons represent the neurons, and the colors within each hexagon represent the neuron's weight vector reshaped into either a specified or automatically determined matrix form. This visualization is useful for analyzing the learned patterns and feature representations within the SOM.
+
+        Parameters
+        ----------
+        rows : int, optional
+            The number of rows to reshape each neuron's weight vector into. If None, the weight vector is reshaped into a square matrix by default. If specified, the weight vector is reshaped into a matrix with the given number of rows, and the number of columns is determined automatically.
+        mouse_click : bool, optional
+            If True, enables the plot to respond to mouse clicks, allowing for interactive functionality such as querying or modifying neuron data, by default False.
+        connect_pick_event : bool, optional
+            If True, connects a pick event that triggers when a neuron is clicked, by default True.
+        **kwargs : dict
+            Arbitrary keyword arguments that can be passed to the event handler onpick when an interactive element is clicked. Common parameters could include data specific to the plot or visualization settings.
+
+        Returns
+        -------
+        fig : matplotlib.figure.Figure
+            The Figure object containing the plot.
+        ax : matplotlib.axes.Axes
+            The Axes object containing the plot elements.
+        patches : list
+            A list of matplotlib.patches.Patch objects, each representing a hexagon in the plot.
+        """
+
         w = self.w  # Weight matrix
         pos = self.pos  # Positions of the neurons
         numNeurons = self.numNeurons  # Number of neurons
 
         # Get the shape of a single hexagon
         shapex, shapey = get_hexagon_shape()
 
@@ -1386,15 +1582,16 @@
 
         # Return the figure components
         return fig, ax, patches
 
     # Generic Plot Function
     def plot(self, plot_type, data_dict=None, ind=None, target_class=None, use_add_array=False,
              **kwargs):
-        """ Generic Plot Function.
+        """
+        Generic Plot Function.
         It generates a plot based on the plot type and data provides.
 
         Parameters
         ----------
         plot_type : str
             The type of plot to be generated:
             ["top", "top_num", "hit_hist", "gray_hist",
@@ -1729,23 +1926,25 @@
             # Call the box plot and violin function
             return selected_plot(x, **kwargs)
 
     # Interactive Functionality
     def onpick(self, event, hexagons, hexagon_to_neuron, **kwargs):
         """
         Interactive Plot Function
-        Args:
-            event: event
-                a mouse click event
-            hexagons: list
-                a list of hexagons
-            hexagon_to_neuron: dict
-                a dictionary mapping hexagons to neurons
-            **kwargs:
 
+        Parameters
+        ----------
+        event: event
+            a mouse click event
+        hexagons: list
+            a list of hexagons
+        hexagon_to_neuron: dict
+            a dictionary mapping hexagons to neurons
+        **kwargs:
+            a dictionary with input data
         Returns:
             None
         """
         if event.artist not in hexagons:
             return
 
         # Detect the clicked hexagon
@@ -1772,21 +1971,21 @@
         for button_type, button in self.buttons.items():
             button.on_clicked(self.create_click_handler(button_type, ax, neuron_ind, **kwargs))
 
         # Show up the 2nd window
         plt.show()
 
     def create_click_handler(self, button_type, ax, neuron_ind, **kwargs):
+        # Generates a custom event handler for button clicks in a plot.
         def handler(event):
             self.button_click_event(button_type, ax, neuron_ind, **kwargs)
 
         return handler
 
     def button_click_event(self, button_type, ax, neuron_ind, **kwargs):
-
         # Handle button click event by calling the appropriate plot function
         if button_type == 'pie':
             # Pre-process categorical variables
             sizes = kwargs['cat']
             sizes = sizes[neuron_ind][:kwargs['topn']]
             self.plot_pie(ax, sizes, neuron_ind)
 
@@ -1830,14 +2029,15 @@
             sub_clust_data = cluster_data[neuron_ind]  # Get the data for the
             self.sub_clustering(sub_clust_data, neuron_ind)
 
         else:
             print(f"Unknown button type: {button_type}")
 
     def determine_button_types(self, **kwargs):
+        # Determine the button type based on the contents of **kwargs
         button_types = []
 
         # Check for categorical data for pie charts
         if 'cat' in kwargs and kwargs['cat'] is not None:
             button_types.append('pie')
             button_types.append('stem')
 
@@ -1857,36 +2057,52 @@
             button_types.append('sub_cluster')
 
         return button_types
 
     # Helper function to create charts
     def plot_pie(self, ax, data, neuronNum):
         """
-        Helper function to plot pie chart in the interactive plots
-        Args:
-            ax:
-            data:
-            neuronNum:
-
-        Returns:
+        Plots a pie chart on the specified matplotlib axes object.
 
+        Parameters
+        ----------
+        ax : matplotlib.axes.Axes
+            The matplotlib axes object where the pie chart will be plotted.
+        data : array-like
+            An array of numeric data which represents the portions of the pie chart.
+        neuronNum : int
+            The neuron number associated with the data, which is used to title the pie chart.
         """
         # Clear the axes
         ax.clear()
         # Pie chart plot logic here
         # Determine the number of colors needed
         num_colors = len(data)
         cmap = cm.get_cmap('plasma', num_colors)
         clrs = [cmap(i) for i in range(num_colors)]
         ax.pie(data, colors=clrs, autopct='%1.1f%%')
         ax.set_title('Pie Chart inside the Cluster ' + str(neuronNum))
         # Redraw the figure
         ax.figure.canvas.draw_idle()
 
     def plot_stem(self, ax, align, height, neuronNum):
+        """
+        Plots a stem plot for a specific neuron's data on the given axes
+
+        Parameters
+        ----------
+        ax : matplotlib.axes.Axes
+            The matplotlib axes object where the stem plot will be drawn.
+        align : array-like
+            The x positions of the stems.
+        height : array-like
+            The y values for each stem, indexed by neuron number.
+        neuronNum : int
+            The index of the neuron for which the plot is being generated.
+        """
         # Clear the axes
         ax.clear()
         # Stem plot
         ax.stem(align, height[neuronNum])  # x: cat, y: data
         ax.set_title('Stem Plot inside the Clluster ' + str(neuronNum))
         # Redraw the figure
         ax.figure.canvas.draw_idle()
@@ -1907,61 +2123,95 @@
         # Histogram plot logic here
         ax.hist(data)
         ax.set_title('Histogram inside the Cluster ' + str(neuronNum))
         # Redraw the figure
         ax.figure.canvas.draw_idle()
 
     def plot_box(self, ax, data, neuronNum):
+        """
+        Generates a box plot for a specific neuron's data on the provided axes.
+
+        Parameters
+        ----------
+        ax : matplotlib.axes.Axes
+            The axes object on which the box plot will be drawn.
+        data : array-like
+            The data array for which the box plot is to be generated.
+        neuronNum : int
+            The neuron index that the data is associated with.
+        """
         # Clear the axes
         ax.clear()
         # Box plot logic here
         ax.boxplot(data)
         ax.set_title("Box plot in the Cluster " + str(neuronNum))
         # Redraw the figure
         ax.figure.canvas.draw_idle()
 
     def plot_violin(self, ax, data, neuronNum):
+        """
+        Displays a violin plot for a specific neuron's data on the provided axes.
+
+        Parameters
+        ----------
+        ax : matplotlib.axes.Axes
+            The axes object where the violin plot will be drawn.
+        data : array-like
+            The data to be used for the violin plot.
+        neuronNum : int
+            The index of the neuron associated with the data.
+        """
         # Clear the axes
         ax.clear()
         # Violin plot logic here
         ax.violinplot(data)
         ax.set_title('Violin Plot inside the Cluster ' + str(neuronNum))
         # Redraw the figure
         ax.figure.canvas.draw_idle()
 
     def plot_scatter(self, ax, num1, num2, neuronNum):
         """
-        Helper function to display scatter plot in the interactive plots
-        Args:
-            ax:
-            data:
-            num1:
-            num2:
-            neuronNum:
-
-        Returns:
+        Plots a scatter plot for a specific neuron's data on the provided axes.
 
+        Parameters
+        ----------
+        ax : matplotlib.axes.Axes
+            The axes object on which the scatter plot will be drawn.
+        num1 : array-like
+            The x coordinates of the data points.
+        num2 : array-like
+            The y coordinates of the data points.
+        neuronNum : int
+            The index of the neuron for which the plot is being generated.
         """
         # Clear the axes
         ax.clear()
         # Scatter plot logic here
         ax.scatter(num1, num2)
         ax.set_title('Scatter Plot inside the Cluster ' + str(neuronNum))
         # Redraw the figure
         ax.figure.canvas.draw_idle()
 
     def sub_clustering(self, data, neuron_ind):
         """
-        Helper function for interactive function which create the sub-cluster
-        Args:
-            data:
-            neuron_ind:
+        Performs sub-clustering on the data associated with a specific neuron within the Self-Organizing Map (SOM).
 
-        Returns:
+        Parameters
+        ----------
+        data : array-like
+            The dataset from which sub-clusters are to be derived. Typically, this is the subset of the overall dataset that
+            has been mapped to the neuron specified by `neuron_ind`.
+        neuron_ind : int
+            The index of the neuron for which sub-clustering is to be performed. This index is used to refer to a specific neuron
+            in the SOM's grid.
 
+        Returns
+        -------
+        list of array-like
+            A list of clusters, where each cluster is an array of data points that form a sub-group within the neuron's data.
         """
         if len(data) <= 1:
             print("There is no enough data to create sub-cluster")
             return
 
         if neuron_ind in self.sub_som:
             print('Sub clustering already done')
```

### Comparing `nnsom-1.7.8/src/NNSOM/som.py` & `nnsom-1.7.9/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.7.8/src/NNSOM/som_gpu.py` & `nnsom-1.7.9/src/NNSOM/som_gpu.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.7.8/src/NNSOM/utils.py` & `nnsom-1.7.9/src/NNSOM/utils.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.7.8/.gitignore` & `nnsom-1.7.9/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.7.8/README.md` & `nnsom-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `nnsom-1.7.8/pyproject.toml` & `nnsom-1.7.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.7.8"
+version = "1.7.9"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Martin Hagan" },
   { name = "Dr. Amir Jafari" },
```

### Comparing `nnsom-1.7.8/PKG-INFO` & `nnsom-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.7.8
+Version: 1.7.9
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Project-URL: Documenation, https://amir-jafari.github.io/SOM/
 Author: Dr. Martin Hagan, Dr. Amir Jafari, Lakshmi Sravya Chalapati, Ei Tanaka
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

