# Count Digits
Write a function that counts the number of digits in an integer.

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
int countDigit(int nVal){
	int count = 1;

	while(nVal > 9){
		count++;
		nVal /= 10;
	}

	return count;
}
```

</details>