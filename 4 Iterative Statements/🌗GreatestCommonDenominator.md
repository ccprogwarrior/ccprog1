# Greatest Common Denominator
Write a function that gets the greatest common denominator of 2 integers

gcd(10, 5) returns 5

gcd(2, 3) returns 1

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
int gcd(int a, int b){
	int i;
	i = (a < b)? a : b;
	
	while(a % i != 0 || b%i!= 0) i--;
	return i;
}

```

</details>
