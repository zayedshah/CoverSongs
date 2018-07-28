# Simplest Gradient Descent

Gradient Descent is the backbone of Machine Learning, Deep Learning and Artificial Intelligence (AI).

This is my attempt at reproducing the most simple gradient descent exercise.

This is to be read is conjunction with the notebook *Simplest Gradient Descent.ipynb*

I have a range of number of between 1 and 10 - this is x. And y - which is double of of the numbers in x.

The relationship between them is y = 2 * x. This is an equation of a straight line y = mx + b where m is the slope and b is the intercept. For the sake of simplicity, I have taken out any intercept so b = 0.

Pretend that we dont know that m = 2. We will use gradient descent to find the value of m.

We begin with m as a random number - in the exercise, it begins with 0.687890. For that the loss is around 66. This loss is what we are trying to optimise in gradient descent. The loss has a quadratic relationship with m, the slope of the original line y = mx.

Gradient Descent allows us to play with m so that we can find at what value of m is the loss minimum. We use calculus for that. 

We notice that at m = 0.687890 and loss of around 66, the slope is around -101. This is telling us that it has negative slope, and we need to increase the value of m to bring it to convergence.

In the next iteration, m has been updated to 1.698215 - notice that it has moved from around 0.6 to 1.69 in just one iteration (our target m is 2, see how quickly it begins to guess where m might be - here is power of gradient descent).

With m at 1.69, loss has dropped dramatically to just around 3.5, and corresponding the slope of the quadratic relationship would have reduced, and begin to flatten. The slope is now at -23. Lesser the number of this slope, less steeper is the slope. Compare this to previous slope at -101, which was suggesting that it was quite steep slope. Imagine climbing a steep mountain.

After this, m is updated after every iteration, and we notice that loss and slope decreases, until at the 10th iteration, m is around 1.99 (very close to 2, which is our target m), loss has gone down to something like 0.0000000002 (in the beginning, the loss was around 66), and slope is -0.000182, which is very close to 0. Slope at 0 means that the line drawn at the tangent to the curve is flat.
