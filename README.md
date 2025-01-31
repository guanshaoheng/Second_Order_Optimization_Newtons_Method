# Second_Order_Optimization_Newtons_Method


# Coding Challenge - Due Date, Thursday June 29th 2017 at 12 PM PST

This weeks challenge is to implement Newton's Method for optimization from scratch yourself in a Jupyter Notebook. You can use a toy dataset. Bonus points are given if you compare your results to a first order optimization technique or use a dataset from [Kaggle](https://www.kaggle.com/datasets). 

## Overview

This is the code for [this](https://youtu.be/UIFMLK2nj_w) video on Youtube by Siraj Raval as part of The Math of Intelligence course. I've got 2 implementations of Newton's Method here. The first is the root finding version, and the other is the optimization version. They are both written in just numpy and scipy. Newton's Method uses the 2nd derivative for optimizing, which hints at a graphs curvature, has better step-wise performance, but is usually outperformed by gradient descent because computing the 2nd derivative is computationally expensive. 

## Dependencies

* numpy
* scipy
* matplotlib

Install dependencies with [pip](https://pip.pypa.io/en/stable/)

## Usage

Just run `python name_of_file` in terminal and it will compile.

## Credits

The credits for this code go to [Dsalaj](https://github.com/dsalaj) and [Dhomola](https://gist.github.com/danielhomola). I've merely created a wrapper to get people started.

## Comparation

```angular2html
NEWTON METHOD: start
NEWTON METHOD: result distance: 8.88178e-16 	 iterationNum: 1
STEEPEST DESCENT: start
STEEPEST DESCENT: result distance: 2.96903e-01 	 iterationNum 27 
NEWTON METHOD: start
NEWTON METHOD: result distance: 3.16345e-03 	 iterationNum: 3
STEEPEST DESCENT: start
STEEPEST DESCENT: result distance: 1.44865e+00 	 iterationNum 101 
```

|Function 1| Function 2|
|---|---|
|![](./Comparation_1.png) | ![](./Comparation_2.png) |

## Conclusion 
The Steepest Descent method performs poor while approaching the object, since the gradient value is very small which will contribute less and less to the optimization process.

The **Newtown Method** uses the gradient and the curvature, the curvature can be used to rescale
the optimization step (the step size is inversely proportional to curvature).
