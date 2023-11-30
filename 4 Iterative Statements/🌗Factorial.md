# Factorial Problem
Create a function that computes for the factorial of n


<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
int factorial(int n){
	int i, factorial = 1;
	for(i=2; i<=n;i++){
		factorial *= i;
	}

	return factorial;
}
```
</details>

<details>
<summary>Answer 2</summary>
<br>

``` c
int factorial(int n){
	int factorial = 1;
	for(n; n > 1; n--){
		factorial *= n;
	}

	return factorial;
}
```
</details>
