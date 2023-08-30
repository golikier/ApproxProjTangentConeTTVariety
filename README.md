# ApproxProjTangentConeTTVariety
An approximate projection onto the tangent cone to the variety of third-order tensors of bounded tensor-train rank

In this repository, the Matlab implementation corresponding to the numerical method proposed in the following paper is given:
C. Vermeylen, G. Olikier, and M. Van Barel (2023). 
An Approximate Projection onto the Tangent Cone to the Variety of Third-Order Tensors of Bounded Tensor-Train Rank. 
In: Nielsen, F., Barbaresco, F. (eds) Geometric Science of Information. GSI 2023. 
Lecture Notes in Computer Science, vol 14071. Springer, Cham. 
https://doi.org/10.1007/978-3-031-38271-0_48
 
The function 'approx_proj_NTC_new.m' implements the pseudo-code in Algorithm 1 of the paper.
The function 'approx_proj_NTC_new_v2.m' is a slightly modified version, which provides a slightly better approximation but, on the other hand, is more computationally expensive. The reason why this version is not included in the paper is due to space limitations.

The following two functions are used to compare the proposed method with:
-'approx_proj_NTC_Kutschan.m', which implements the approximate projection defined in 
Kutschan B., Convergence of Gradient Methods on Hierarchical Tensor Varieties, TU Berling, 2018 (PhD thesis).
-'benchmark_proj_NTC.mrk_proj_NTC.m', which uses the build-in Matlab function fmincon to solve the constrained optimization problem (equation 3) in the paper.

The script 'compare_angle_conditions.m', implements the numerical experiment described in Section 4 of the paper and uses the four functions described above.

The data file 'results_rng1-50.mat' contains the data obtained from the experiment in the script and is visualized in Figure 1 of the paper.
 
The other files are auxiliary functions or data and for some functions a short description is given in the header. 



