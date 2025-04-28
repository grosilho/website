---
title: Publications
image: /uploads/photos/article.png
summary: A complete list of all my publications, with descriptions and links to PDF and codes developed.
weight: 1
---

{{< brick_title >}}

![]()   

# Publications

A comprehensive list of my publications, including titles, journals, abstracts, and links to the published articles (<img src="/img/doi.svg" alt="pdf" style="display: inline; width: 1.0rem; height: 1.0rem; margin: 0rem 0rem -0.15rem 0rem"/>), corresponding arXiv preprints (<img src="/img/arxiv.svg" alt="pdf" style="display: inline; width: 1.0rem; height: 1.0rem; margin: 0rem 0rem -0.15rem 0rem"/>), and source code used for generating the results (<img src="/img/github-mark.svg" alt="pdf" style="display: inline; width: 1.0rem; height: 1.0rem; margin: 0rem 0rem -0.15rem 0rem"/>).

<!-- {{< breadcrumbs >}} -->

{{< /brick_title >}}

{{< brick_wide >}}
{{< publication 
"High-order parallel-in-time method for the monodomain equation in cardiac electrophysiology" 
"Giacomo Rosilho de Souza, Simone Pezzuto, and Rolf Krause"
"Submitted to SIAM Journal on Scientific Computing."
>}}
<ul class="mybuttons">
        <li><a href="http://arxiv.org/abs/2405.19994" class="button myicon"><img src="/img/arxiv.svg" alt="arxiv" /></a></li>
        <li><a href="https://github.com/grosilho/pySDC" class="button myicon"><img src="/img/github-mark.svg" alt="github" /></a></li>
</ul>
<div style="font-size: 0.9em;">
Simulation of the monodomain equation, crucial for modeling the heart’s electrical activity, faces scalability limits when traditional numerical methods only parallelize in space. To optimize the use of large multi-processor computers by distributing the computational load more effectively, time parallelization is essential. We introduce a high-order parallel-in-time method addressing the substantial computational challenges posed by the stiff, multiscale, and nonlinear nature of cardiac dynamics. Our method combines the semi-implicit and exponential spectral deferred correction methods, yielding a hybrid method that is extended to parallel-in-time employing the PFASST framework. We thoroughly evaluate the stability, accuracy, and robustness of the proposed parallel-in-time method through extensive numerical experiments, using stateof-the-art ionic models. The results underscore the method’s potential to significantly enhance real-time and high-fidelity simulations in biomedical research and clinical applications.
</div>
{{< /brick_wide >}}


{{< brick_wide >}}
{{< publication 
"Boundary integral formulation of the cell-by-cell model of cardiac electrophysiology"
"Giacomo Rosilho de Souza, Rolf Krause, and Simone Pezzuto"
"Engineering Analysis with Boundary Elements 158 (2024): 239–51."
>}}
<ul class="mybuttons">
        <li><a href="https://doi.org/10.1016/j.enganabound.2023.10.021" class="button myicon"><img src="/img/doi.svg" alt="DOI" /></a></li>
        <li><a href="https://arxiv.org/abs/2302.05281" class="button myicon"><img src="/img/arxiv.svg" alt="arxiv" /></a></li>
        <li><a href="https://github.com/grosilho/BEMI" class="button myicon"><img src="/img/github-mark.svg" alt="github" /></a></li>
</ul>
<div style="font-size: 0.9em;">
We propose a boundary element method for the accurate solution of the cell-by-cell bidomain model of electrophysiology. The cell-by-cell model, also called Extracellular-Membrane-Intracellular (EMI) model, is a system of reaction-diffusion equations describing the evolution of the electric potential within each domain: intra- and extra-cellular space and the cellular membrane. The system is parabolic but degenerate because the time derivative is only in the membrane domain. In this work, we adopt a boundary-integral formulation for removing the degeneracy in the system and recast it to a parabolic equation on the membrane. The formulation is also numerically advantageous since the number of degrees of freedom is sensibly reduced compared to the original model. Specifically, we prove that the boundary-element discretization of the EMI model is equivalent to a system of ordinary differential equations, and we consider a time discretization based on the multirate explicit stabilized Runge-Kutta method. We numerically show that our scheme convergences exponentially in space for the single-cell case. We finally provide several numerical experiments of biological interest.
</div>
{{< /brick_wide >}}


{{< brick_wide >}}
{{< publication 
"Explicit stabilized multirate methods for the monodomain model in cardiac electrophysiology"
"Giacomo Rosilho de Souza, Marcus Grote, Simone Pezzuto, and Rolf Krause"
"ESAIM: Mathematical Modelling and Numerical Analysis, 2024."
>}}
<ul class="mybuttons">
        <li><a href="https://doi.org/10.1051/m2an/2024030" class="button myicon"><img src="/img/doi.svg" alt="DOI" /></a></li>
        <li><a href="https://arxiv.org/abs/2401.01745" class="button myicon"><img src="/img/arxiv.svg" alt="arxiv" /></a></li>
        <li><a href="https://github.com/grosilho/emRKC" class="button myicon"><img src="/img/github-mark.svg" alt="github" /></a></li>
</ul>
<div style="font-size: 0.9em;">
Fully explicit stabilized multirate (mRKC) methods are well-suited for the numerical solution of large multiscale systems of stiff ordinary differential equations thanks to their improved stability properties. To demonstrate their efficiency for the numerical solution of stiff, multiscale, nonlinear parabolic PDE's, we apply mRKC methods to the monodomain equation from cardiac electrophysiology. In doing so, we propose an improved version, specifically tailored to the monodomain model, which leads to the explicit exponential multirate stabilized (emRKC) method. Several numerical experiments are conducted to evaluate the efficiency of both mRKC and emRKC, while taking into account different finite element meshes (structured and unstructured) and realistic ionic models. The new emRKC method typically outperforms a standard implicit-explicit baseline method for cardiac electrophysiology. Code profiling and strong scalability results further demonstrate that emRKC is faster and inherently parallel without sacrificing accuracy.
</div>
{{< /brick_wide >}}


{{< brick_wide >}}
{{< publication 
"Optimal explicit stabilized postprocessed τ-leap method for the simulation of chemical kinetics"
"Assyr Abdulle, Lia Gander, and Giacomo Rosilho de Souza"
"Journal of Computational Physics, 2023, 112482."
>}}
<ul class="mybuttons">
        <li><a href="https://doi.org/10.1016/j.jcp.2023.112482" class="button myicon"><img src="/img/doi.svg" alt="DOI" /></a></li>
        <li><a href="https://arxiv.org/abs/2106.09339" class="button myicon"><img src="/img/arxiv.svg" alt="arxiv" /></a></li>
        <li><a href="https://github.com/grosilho/sk-tau-rock_methods" class="button myicon"><img src="/img/github-mark.svg" alt="github" /></a></li>
</ul>
<div style="font-size: 0.9em;">
The simulation of chemical kinetics involving multiple scales constitutes a modeling challenge (from ordinary differential equations to Markov chain) and a computational challenge (multiple scales, large dynamical systems, time step restrictions). In this paper we propose a new discrete stochastic simulation algorithm: the postprocessed second kind stabilized orthogonal τ-leap Runge-Kutta method (PSK-τ-ROCK). In the context of chemical kinetics this method can be seen as a stabilization of Gillespie's explicit τ-leap combined with a postprocessor. The stabilized procedure allows to simulate problems with multiple scales (stiff), while the postprocessing procedure allows to approximate the invariant measure (e.g. mean and variance) of ergodic stochastic dynamical systems. We prove stability and accuracy of the PSK-τ-ROCK. Numerical experiments illustrate the high reliability and efficiency of the scheme when compared to other τ-leap methods
</div>
{{< /brick_wide >}}


{{< brick_wide >}}
{{< publication
"Effect of Gap Junction Distribution, Size, and Shape on the Conduction Velocity in a Cell-by-Cell Model for Electrophysiology"
"Giacomo Rosilho de Souza, Simone Pezzuto, and Rolf Krause"
"In Functional Imaging and Modeling of the Heart, 117–26. Springer Nature Switzerland, 2023."
>}}
<ul class="mybuttons">
        <li><a href="https://doi.org/10.1007/978-3-031-35302-4_12" class="button myicon"><img src="/img/doi.svg" alt="DOI" /></a></li>
        <li><a href="https://github.com/grosilho/BEMI" class="button myicon"><img src="/img/github-mark.svg" alt="github" /></a></li>
</ul>
<div style="font-size: 0.9em;">
Gap junction arrangement is a major determinant of cardiac conduction velocity. Importantly, structural remodeling of the myocardium may lead to pathological CV and a pro-arrhythmic substrate. In this work we aim at quantifying the side-to-side conduction velocity in a sub-micrometer model of the myocardium that accounts for gap junctions. We consider the Extracellular-Membrane-Intracellular (EMI) model, which describes the evolution of the electric potential within each cell and in the extracellular space. For the solution of the model, we propose a boundary integral formulation of the cell-to-cell model that leads to small system of ODEs. We study several configurations of lateral gap junction distribution, as well as different shapes and sizes of the cell-to-cell connection. We find that irregular positioning of gap junctions from cell to cell is of utmost importance to obtain realistic CV values, while gap junction’s shape is of secondary importance.
</div>
{{< /brick_wide >}}


{{< brick_wide >}}
{{< publication
"Mixed-precision explicit stabilized Runge-Kutta methods for single- and multi-scale differential equations"
"Matteo Croci and Giacomo Rosilho de Souza"
"Journal of Computational Physics 464 (2022)."
>}}
<ul class="mybuttons">
        <li><a href="https://doi.org/10.1016/j.jcp.2022.111349" class="button myicon"><img src="/img/doi.svg" alt="DOI" /></a></li>
        <li><a href="https://arxiv.org/abs/2109.12153" class="button myicon"><img src="/img/arxiv.svg" alt="arxiv" /></a></li>
</ul>
<div style="font-size: 0.9em;">
Mixed-precision algorithms combine low- and high-precision computations in order to benefit from the performance gains of reduced-precision without sacrificing accuracy. In this work, we design mixed-precision Runge-Kutta-Chebyshev (RKC) methods, where high precision is used for accuracy, and low precision for stability. Generally speaking, RKC methods are low-order explicit schemes with a stability domain growing quadratically with the number of function evaluations. For this reason, most of the computational effort is spent on stability rather than accuracy purposes. In this paper, we show that a naïve mixed-precision implementation of any Runge-Kutta scheme can harm the convergence order of the method and limit its accuracy, and we introduce a new class of mixed-precision RKC schemes that are instead unaffected by this limiting behaviour. We present three mixed-precision schemes: a first- and a second-order RKC method, and a first-order multirate RKC scheme for multiscale problems. These schemes perform only the few function evaluations needed for accuracy (1 or 2 for first- and second-order methods respectively) in high precision, while the rest are performed in low precision. We prove that while these methods are essentially as cheap as their fully low-precision equivalent, they retain the stability and convergence order of their high-precision counterpart. Indeed, numerical experiments confirm that these schemes are as accurate as the corresponding high-precision method.
</div>
{{< /brick_wide >}}


{{< brick_wide >}}
{{< publication
"Explicit stabilized multirate method for stiff stochastic differential equations"
"Assyr Abdulle and Giacomo Rosilho de Souza"
"SIAM Journal on Scientific Computing 44, fasc. 4 (2022): A1859–83."
>}}
<ul class="mybuttons">
        <li><a href="https://doi.org/10.1137/21M1439018" class="button myicon"><img src="/img/doi.svg" alt="DOI" /></a></li>
        <li><a href="https://arxiv.org/abs/2010.15193" class="button myicon"><img src="/img/arxiv.svg" alt="arxiv" /></a></li>
        <li><a href="https://github.com/grosilho/SK-mROCK" class="button myicon"><img src="/img/github-mark.svg" alt="github" /></a></li>
</ul>
<div style="font-size: 0.9em;">
Stabilized explicit methods are particularly efficient for large systems of stiff stochastic differential equations (SDEs) due to their extended stability domain. However, they loose their efficiency when a severe stiffness is induced by very few "fast" degrees of freedom, as the stiff and nonstiff terms are evaluated concurrently. Therefore, inspired by [A. Abdulle, M. J. Grote, and G. Rosilho de Souza, Preprint (2020), arXiv:2006.00744] we introduce a stochastic modified equation whose stiffness depends solely on the "slow" terms. By integrating this modified equation with a stabilized explicit scheme we devise a multirate method which overcomes the bottleneck caused by a few severely stiff terms and recovers the efficiency of stabilized schemes for large systems of nonlinear SDEs. The scheme is not based on any scale separation assumption of the SDE and therefore it is employable for problems stemming from the spatial discretization of stochastic parabolic partial differential equations on locally refined grids. The multirate scheme has strong order 1/2, weak order 1 and its stability is proved on a model problem. Numerical experiments confirm the efficiency and accuracy of the scheme.
</div>
{{< /brick_wide >}}


{{< brick_wide >}}
{{< publication
"A local adaptive discontinuous Galerkin method for convection-diffusion-reaction equations"
"Assyr Abdulle and Giacomo Rosilho de Souza"
"Journal of Computational Physics 451 (2022)."
>}}
<ul class="mybuttons">
        <li><a href="https://doi.org/10.1016/j.jcp.2021.110894" class="button myicon"><img src="/img/doi.svg" alt="DOI" /></a></li>
        <li><a href="https://arxiv.org/abs/2004.07148" class="button myicon"><img src="/img/arxiv.svg" alt="arxiv" /></a></li>
</ul>
<div style="font-size: 0.9em;">
We introduce a local adaptive discontinuous Galerkin method for convection-diffusion-reaction equations. The proposed method is based on a coarse grid and iteratively improves the solution's accuracy by solving local elliptic problems in refined subdomains. For purely diffusion problems, we already proved that this scheme converges under minimal regularity assumptions [A. Abdulle and G.Rosilho de Souza, ESAIM: M2AN, 53(4):1269--1303, 2019]. In this paper, we provide an algorithm for the automatic identification of the local elliptic problems' subdomains employing a flux reconstruction strategy. Reliable error estimators are derived for the local adaptive method. Numerical comparisons with a classical nonlocal adaptive algorithm illustrate the efficiency of the method.
</div>
{{< /brick_wide >}}


{{< brick_wide >}}
{{< publication
"Explicit stabilized multirate method for stiff differential equations"
"Assyr Abdulle, Marcus Grote, and Giacomo Rosilho de Souza"
"Mathematics of Computation 91, fasc. 338 (2022): 2681–2714."
>}}
<ul class="mybuttons">
        <li><a href="https://doi.org/10.1090/mcom/3753" class="button myicon"><img src="/img/doi.svg" alt="DOI" /></a></li>
        <li><a href="https://arxiv.org/abs/2006.00744" class="button myicon"><img src="/img/arxiv.svg" alt="arxiv" /></a></li>
        <li><a href="https://github.com/grosilho/mRKC" class="button myicon"><img src="/img/github-mark.svg" alt="github" /></a></li>
</ul>
<div style="font-size: 0.9em;">
Stabilized Runge-Kutta methods are especially efficient for the numerical solution of large systems of stiff nonlinear differential equations because they are fully explicit. For semi-discrete parabolic problems, for instance, stabilized Runge-Kutta methods overcome the stringent stability condition of standard methods without sacrificing explicitness. However, when stiffness is only induced by a few components, as in the presence of spatially local mesh refinement, their efficiency deteriorates. To remove the crippling effect of a few severely stiff components on the entire system of differential equations, we derive a modified equation, whose stiffness solely depend on the remaining mildly stiff components. By applying stabilized Runge-Kutta methods to this modified equation, we then devise an explicit multirate Runge-Kutta-Chebyshev (mRKC) method whose stability conditions are independent of a few severely stiff components. Stability of the mRKC method is proved for a model problem, whereas its efficiency and usefulness are demonstrated through a series of numerical experiments.
</div>
{{< /brick_wide >}}


{{< brick_wide >}}
{{< publication
"A local discontinuous Galerkin gradient discretization method for linear and quasilinear elliptic equations"
"Assyr Abdulle and Giacomo Rosilho de Souza"
"ESAIM: Mathematical Modelling and Numerical Analysis 53, fasc. 4 (2019): 1269–1303."
>}}
<ul class="mybuttons">
        <li><a href="https://doi.org/10.1051/m2an/2019022" class="button myicon"><img src="/img/doi.svg" alt="DOI" /></a></li>
        <li><a href="https://arxiv.org/abs/1807.10645" class="button myicon"><img src="/img/arxiv.svg" alt="arxiv" /></a></li>
</ul>
<div style="font-size: 0.9em;">
A local weighted discontinuous Galerkin gradient discretization method for solving elliptic equations is introduced. The local scheme is based on a coarse grid and successively improves the solution solving a sequence of local elliptic problems in high gradient regions. Using the gradient discretization framework we prove convergence of the scheme for linear and quasilinear equations under minimal regularity assumptions. The error due to artificial boundary conditions is also analyzed, shown to be of higher order and shown to depend only locally on the regularity of the solution. Numerical experiments illustrate our theoretical findings and the local method's accuracy is compared against the non local approach
</div>
{{< /brick_wide >}}


{{< brick_wide >}}
{{< publication
"Numerical methods for deterministic and stochastic differential equations with multiple scales and high contrasts"
"Giacomo Rosilho de Souza"
"PhD thesis"
>}}
<ul class="mybuttons">
        <li><a href="https://doi.org/10.5075/epfl-thesis-7445" class="button myicon"><img src="/img/doi.svg" alt="DOI" /></a></li>
</ul>
<div style="font-size: 0.9em;">
Mathematical models involving multiple scales are essential for the description of physical systems. In particular, these models are important for the simulation of time-dependent phenomena, such as the heat flow, where the Laplacian contains mixed and indistinguishable fast and slow modes. Stationary problems can also exhibit a multiscale nature. For example, elliptic equations governed by a diffusion coefficient with strong discontinuities have solutions characterized by regions with a high gradient. Simulating such models is very demanding, as the computational cost of standard numerical methods is usually ruled by the fastest dynamics or the smallest scale.
<br>
In the first part of this thesis, we develop multirate integration methods for deterministic and stochastic time-dependent problems with disparate time-scales. The cost of traditional schemes for such problems is prohibitive due to step size restrictions in the explicit case or solutions to large nonlinear systems in the implicit case. Existing multirate methods are either implicit or make use of interpolations, which trigger instabilities, or are based on a scale separation assumption, which is not satisfied by parabolic problems. Here we introduce a new framework based on modified equations which allows for the development of a whole new class of interpolation-free explicit multirate numerical methods, which do not need any scale separation, are stable and accurate. For deterministic problems, our methodology is based on the replacement of the original right-hand side by an averaged force, whose stiffness is reduced due to a fast but cheap auxiliary problem. Integrating the modified equation and the auxiliary problems by explicit schemes is generally cheaper than integrating the original problem. We thus introduce a multirate method based on stabilized explicit schemes and prove its efficiency, stability and accuracy. Numerical experiments show that standard schemes and our multirate approach provide essentially the same solutions; hence, the bottleneck caused by the stiffness of a few degrees of freedom is overcome without sacrificing accuracy. We also generalize the same framework to stochastic differential equations, where we need to introduce a damped diffusion term for which the resulting modified equation inherits the mean-square stability properties of the original problem. An interpolation-free stabilized explicit multirate method for stochastic equations is then derived.
<br>
In the second part of this thesis, we consider elliptic problems with high gradients and develop a local adaptive discontinuous Galerkin scheme. Local methods for such problems already exist in literature; however, they are usually based on iterations and have several downsides. In particular, their a priori error analysis is based on rather strong and nonphysical assumptions and they lack a rigorous a posteriori error analysis. The scheme that we propose is based on a coarse solution on the full domain which is subsequently improved by solving local elliptic problems only once on subdomains with artificial boundary conditions. The a priori error analysis is performed under minimal regularity assumptions due to the gradient discretization framework. Furthermore, we derive a posteriori error estimators based on conforming fluxes and potential reconstructions which can be used to identify the local subdomains on the fly, are free of undetermined constants and robust in singularly perturbed regimes.
</div>
{{< /brick_wide >}}


