# PECo
PECo: A Point-edge Collaborative Framework for Global-aware Urban Building Contouring from Unstructured Point Clouds.
We cast the maximization problems as the MST problem, 
the E-step of our EM algorithm amounts to a summation of the probabilities as weights for each edge, 
whereas the M-step is to iteratively solve the MST problem in the ICM framework. e 
# Why do we propose a point-edge collaborative framework for global-aware urban building contouring (PECo)?
It operates on the observations that while contour points are sensitive to local point clouds, they can be made more robust by introducing contour edge information, which covers a broader area of the building's surface.
Conversely, the global relationship of contour edges can benefit from improved contour points that are less susceptible to noise and incomplete point cloud data. 
Thus, the PECo contouring method combines the point and edge domains to enhance building contouring.
# Pipline
The pipeline of our proposed PECo: point-edge collaborative framework for global-aware urban building contouring. 
The point clouds (a) of the building are input to obtain the building contours. 
The initial probability of the point cloud (b) is estimated based on the local shape descriptors to obtain rough contour points.
After that, the building contouring is performed via an expectation maximization (EM) iteration procedure (c). 
In the E-step, the updated probability of the point clouds labeled as contour points and the expectation over this probability is estimated. 
Coupling with this probability, in the M-step, the contour edges are inferred by considering the global structure of the contouring. 
The contours are progressively refined in EM iterations. This leads to robust and high-fidelity building contouring results when the iteration converges (d).
![image](https://github.com/DAPointcloud/PECo/assets/145087751/13b60d3b-d218-40ee-b77c-04ba5e1fc022)
![image](https://github.com/DAPointcloud/PECo/assets/145087751/37842249-9551-4542-b4ac-39331acb515b)
