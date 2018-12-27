# Graph Extractor
(Very) preliminary Python code to extract a weighted graph from thinned images (similar to NEFI).

The image is first thinned to obtain a "quasi-1D" appearance and then it is convoluted with several matrix kernels, each one identifying leaves and many kinds of intersections.

Hope to clean up the code and add some more comments, but the notebook should be quite self explanatory and easy to use.

In the first part of the notebook I set up the Python functions to build the graph, then the image is loaded, color images get transformed to BW, the levels are equalized by choosing specific thresholds and then we proceed to thin it with standard routines.
The output object is a NetworkX undirected, weighted graph ready to analyze as you want.

Being based on Numpy convolution functions, the most CPU intensive stuff is automatically distributed among all your cores, and it scales pretty well.

Have fun!

marco
