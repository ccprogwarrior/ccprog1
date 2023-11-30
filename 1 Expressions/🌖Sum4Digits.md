# 3-Digit Integer Components
Write a program that adds the digits of a 4-digit integer.

If val = 1234 output:
```
sum = 10
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
	int n, first, second, third, fourth, sum;
	n = 1234;
	first = n / 1000;
	second = n / 100 % 10;
	third = n / 10 % 10;
	fourth = n % 10;
	sum = first+second+third+fourth;
	printf("sum=%d\n", sum);
	return 0;
}
```

</details>
