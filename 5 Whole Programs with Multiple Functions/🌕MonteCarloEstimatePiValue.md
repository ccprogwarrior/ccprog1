# Monte Carlo Estimate Value of Pi

The Monte Carlo method for estimating pi is based on the idea that if you randomly scatter points inside a square and count the number of points that fall inside a circle inscribed in the square, you can estimate the value of pi. The algorithm for this method is straightforward:

1. Generate a random point (x, y) inside a square of side 2 centered at the origin.

2. Determine whether the point falls inside the unit circle inscribed in the square by checking whether x² + y² <= 1.

3. Repeat steps 1 and 2 for a large number of points (e.g., 10⁷).

4. Calculate the ratio of the number of points that fell inside the circle to the total number of points generated.

5. Multiply the ratio by 4 to estimate the value of pi.

https://medium.com/the-modern-scientist/estimating-pi-using-monte-carlo-methods-dbdf26c888d6#:~:text=The%20Monte%20Carlo%20method%20for%20estimating%20pi%20is%20based%20on,estimate%20the%20value%20of%20pi.

<details>
<summary>Answer</summary>
<br>

``` c
#include<stdio.h>
#include<stdlib.h>
#include<math.h>

int
isInCricle(double x, double y, double radius){
	return sqrt(pow(x,2) + pow(y,2)) <= radius;
}

double
getEstPiVal(int nTries){
	int i, nCirclePtCount;
	double x, y, dEstPiVal;
	nCirclePtCount = 0;
	for(i=0; i< nTries; i++){
		x = rand() / (RAND_MAX * 1.0);
		y = rand() / (RAND_MAX * 1.0);
		if(isInCricle(x, y, 1)){
			nCirclePtCount ++;
		}
	}

	dEstPiVal = nCirclePtCount / (nTries * 1.0) * 4;
	return dEstPiVal;
}

int
main(){
	srand(10);
	printf("Estimated value of pi: %f", getEstPiVal(1000000));
	return 0;
}
```

</details>
