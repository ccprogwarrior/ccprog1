# Add Digits
Write a function that adds the number of digits of an integer.

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
int addDigits(int nVal){
	int sum = 0;
	while(nVal > 0){
		sum += nVal % 10;
		nVal /= 10;
	}
	
	return sum;
}
```

</details>
