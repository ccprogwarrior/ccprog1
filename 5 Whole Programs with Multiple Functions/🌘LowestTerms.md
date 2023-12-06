# Fraction Lowest Term Problem
Write a function that gets the lowest term of a fraction.

A fraction is at its lowest term if the GCD of its numerator and denominator is 1.

Example

2 / 10 lowest term is 1 / 5

7 / 8 is already in lowest term

9 / 30 lowest term is 3 / 10

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
int 
getgcd(int a, int b){ //copied from greatest common denominator problem
	int i;
	i = (a < b)? a : b;

	while(a % i != 0 || b%i!= 0) i--;
	return i;
}


void
lowestterm(int * num, int * den){
	int gcd;
	while(getgcd(*num, *den) != 1){
		gcd = getgcd(*num, *den);
		*num /= gcd;
		*den /= gcd;
	}

}
```

</details>
