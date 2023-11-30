# isPrime Integer Problem
Write a function that determines if an integer is a prime

Note a prime number is a whole number greater than 1 whose only factors are 1 and itself

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
int isPrime(int n){
	int i, prime = 1;

	for(i=2;i<n;i++){
		if(n%i==0)
			prime = 0;
	}

	return prime;
}
```

</details>
