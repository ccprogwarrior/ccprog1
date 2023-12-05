# QuadraticFormula Problem
Write a function that computes for the roots of a 
quadratic equation using the quadratic formula. Given the coefficients of a quadratic formula as input.


![Quadratic Formula](https://cdn1.byjus.com/wp-content/uploads/2022/02/Quadratic-Formula.png "Quadratic Formula")


Hint: use sqrt and pow function of math.h

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
void 
quadraticFormula(int a, int b, int c, int * x1, int * x2){
	*x1 = (-b + sqrt(pow(b,2) - 4 * a * c)) / (2.0 * a);
	*x2 = (-b - sqrt(pow(b,2) - 4 * a * c)) / (2.0 * a);
}

```

</details>
