# Gradient-Descent
Finding the local minima of the function y=(x+5)² starting from the point x=3


Solution : We know the answer just by looking at the graph. y = (x+5)² reaches it’s minimum value when x = -5 (i.e when x=-5, y=0). Hence x=-5 is the local and global minima of the function.
Now, let’s see how to obtain the same numerically using gradient descent.
Step 1 : Initialize x =3. Then, find the gradient of the function, dy/dx = 2*(x+5).
Step 2 : Move in the direction of the negative of the gradient (Why?). But wait, how much to move? For that, we require a learning rate. Let us assume the learning rate → 0.01
Step 3 : Let’s perform 2 iterations of gradient descent

Step 4 : We can observe that the X value is slowly decreasing and should converge to -5 (the local minima). However, how many iterations should we perform?
Let us set a precision variable in our algorithm which calculates the difference between two consecutive “x” values . If the difference between x values from 2 consecutive iterations is lesser than the precision we set, stop the algorithm !
