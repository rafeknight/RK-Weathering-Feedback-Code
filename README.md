# RK-Weathering-Feedback-Code
The feedback model is an idealized Bayesian model that uses Turing.jl (version 0.43) for MCMC and largely follows Turing's Bayesian differential equations tutorial: https://turinglang.org/docs/tutorials/bayesian-differential-equations/.
An in-depth description of all aspects of the model (including parameters and the formulation of the random walks) can be found in the methods section and the appendix of the corresponding paper.

**Model Files:**

The file named "Base Case" represents the standard formulation of the model

The file named "Increased Uncertainties" represents the model formulation where CenCO2PIP uncertainties are doubled 

The file named "Constant Weathering Sensitivity" represents the model formulation where wT is constant

The file named "Other Forcing Random Walk" represents the model formulation where O is allowed to vary as a random walk

**Plots File:**

The model exports posterior parameters (for each time step). To create each plot, the random walks must be recreated from the posteriors, which is done in the file named "Final Plots".

**Data Files**

The Data required for the model and  plotting is as follows:
CenCO2PIP data converted to doublings: "cenco2pip_500kyr_testrev_ppm"
