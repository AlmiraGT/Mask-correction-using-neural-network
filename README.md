# Mask-correction-using-neural-network

Optical proximity correction (OPC) is one of the resolution enhancement techniques (RETs) in optical lithography, where the mask pattern is modified to improve the output pattern fidelity. 

During optical proximity correction, the boundaries of polygons are divided into fragments in a predetermined way. Then the contour of the image obtained in the photoresistive mask is modeled. Next, for each fragment the distance between contour and initial fragment is determined. Then the offset is being made. And this cycle repeats several times until the error becomes less than a certain threshold.

Due to the decrease of minimal topological norm, the number of iterations required for convergence increases, therefore, the simulation time increases. Therefore, in my task of determining fragments shifts, it makes sense to use machine learning-based methods, or ML-OPC, to speed up calculations.

My goal was to find out whether initial image addition would make neural network prediction more accurate.

**First neural network:**
Input matrix: fragments of aerial images of topology.
Output: list of fragments shifts.

**Second neural network:**
Input matrics: pairs (aerial image, initial images) of fragments.
Output: list of fragments shifts.

As a result we see that the second neural network is more accurate.