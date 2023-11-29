# Get Digit At Place
Write a function that gets the nth digit of an integer. Assuming that the rightmost digit is 1.

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
int getDigitFromRight(int val, int place){
	int i;
	for(i=1; i<place; i++){
		val/=10;
	}
	return val%10;
}
```

</details>