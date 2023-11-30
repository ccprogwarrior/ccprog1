# Four Digit Palindrome Problem
Create a function that determines if a four digit integer is a palindrome or not

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
int isPalindrome(int n){

	int d1, d2, d3, d4;
	d1 = n / 1000;
	d2 = n / 100 % 10;
	d3 = n / 10 % 10
	d4 = n % 10;

	return d1 == d4 && d2 == d3;

}
```
</details>