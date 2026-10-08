# Estimation Theory and Sensor Fusion

I completed this graduate-level coursework at Sharif University of Technology under Professor Behzad Ahi, earning a final course grade of **17.5/20**. The official course title was **Inertial Navigation**; this repository title describes the estimation and sensor-fusion topics represented in the selected work.

## Selected coursework

I selected **Assignment 6** as a representative sample because it brings together stochastic modeling, nonlinear state estimation, multi-rate sensor fusion, and quantitative evaluation of estimation algorithms. It demonstrates my implementation and analysis of these methods through simulated systems, rather than serving as a complete archive of the course.

In this assignment, I:

- Generated correlated Gaussian random vectors using matrix square roots, Cholesky factorization, and eigendecomposition, and checked their empirical covariance and process/measurement cross-covariance.
- Implemented an extended Kalman filter for a planar mobile robot with range and bearing measurements arriving at different rates. I examined initialization error, uncertainty envelopes, measurement outages, and compensation for delayed measurements.
- Implemented and compared EKF, square-root unscented Kalman filtering (SRUKF), and square-root cubature Kalman filtering (SRCKF) for a noisy Van der Pol oscillator, using 130 Monte Carlo trials, RMSE, a posterior Cramer–Rao lower-bound calculation, and runtime measurements.

## Report and implementation

[Read my submitted report](selected-coursework-report.pdf). The 72-page report includes mathematical derivations, MATLAB listings, simulation figures, numerical results, and my discussion of the accuracy–computation tradeoff. The data for the illustrated systems are generated within the simulation code.

This is a coursework submission, not an independent research project. I have retained the report as submitted. The MATLAB listings have not been independently rerun for this repository; on page 2, the covariance-ranking expression refers to an undefined variable named `Hardcoded`, which should be checked against the intended target covariance `Q` before reproducing that part. Local output paths in the listings also need adapting to the reader's environment.
