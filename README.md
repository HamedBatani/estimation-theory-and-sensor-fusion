# Estimation Theory and Sensor Fusion

My selected graduate-level coursework in estimation theory and sensor fusion covers stochastic modeling, nonlinear state estimation, and quantitative evaluation of filtering methods. I completed the course at Sharif University of Technology under Professor Behzad Ahi, earning **17.5/20**. Official course title: **Inertial Navigation**.

## Selected coursework

I implemented and evaluated correlated-noise models, multi-rate sensor fusion, and nonlinear filters in MATLAB using a planar mobile robot and a Van der Pol oscillator. My analysis examines estimation accuracy, uncertainty, measurement interruptions and delays, and computational cost.

In this work, I:

- Generated correlated Gaussian random vectors using matrix square roots, Cholesky factorization, and eigendecomposition, and checked their empirical covariance and process/measurement cross-covariance.
- Implemented an extended Kalman filter for a planar mobile robot with range and bearing measurements arriving at different rates. I examined initialization error, uncertainty envelopes, measurement outages, and compensation for delayed measurements.
- Implemented and compared EKF, square-root unscented Kalman filtering (SRUKF), and square-root cubature Kalman filtering (SRCKF) for a noisy Van der Pol oscillator, using 130 Monte Carlo trials, RMSE, a posterior Cramer–Rao lower-bound calculation, and runtime measurements.

## Report and implementation

[Read my submitted report](selected-coursework-report.pdf). The 72-page report includes mathematical derivations, MATLAB listings, simulation figures, numerical results, and my discussion of the accuracy–computation tradeoff. The data for the illustrated systems are generated within the simulation code.

### Reproduction notes

The report is preserved as submitted. The MATLAB listings have not been independently rerun for this repository; on page 2, the covariance-ranking expression refers to an undefined variable named `Hardcoded`, which should be checked against the intended target covariance `Q` before reproducing that part. Local output paths in the listings also need adapting to the reader's environment.
