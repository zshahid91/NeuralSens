# cran-comments.md

## Add `inp_var` argument in plotting functions 
In some use cases there are too many variables in the plotting functions to be useful. This argument
allows to choose which variables shall be plotted.

## donttest{} examples

The `SensAnalysisMLP.R` function contains `\donttest{}` examples which produce animations that take >5sec that users need to know about, but cause issues in examples and checks. The `HessianMLP.R` function contains `\donttest{}` examples which produce animations that take >5sec that users need to know about, but cause issues in examples and checks. 
The manipulations before the animation rending is already tested in the examples which are not wrapped by `\donttest{}`.

## Test environments
* Windows 10 Home x64, R 4.3.0
* Ubuntu Linux 22.04 LTS, R-release, GCC (r-hub)
* Fedora Linux, R-devel, clang, gfortran (r-hub)
* win-builder, R (oldrelease, release and devel)

### R CMD check
── R CMD check results ─────── NeuralSens 1.0.2 ────
Duration: 6m 41.6s

0 errors ✔ | 0 warnings ✔ | 0 notes ✔

R CMD check succeeded

## win-builder
- oldrelease pass
- release pass
- devel pass


