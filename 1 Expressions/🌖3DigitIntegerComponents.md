# 3-Digit Integer Components
Write a program that splits a given 3-digit integer to its digits using expressions.

If val = 123 output:
```
1
2
3
```

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
int main(){
	int n = 123;
	printf("%d\n", n / 100);
	printf("%d\n", n / 10 % 10);
	printf("%d", n % 10);

	return 0;
}
```

</details>
