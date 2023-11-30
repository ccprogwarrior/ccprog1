# Multiplication Table Problem
Display an n x n multiplication table.

For example, if n = 5:
```
1  2  3  4  5
2  4  6  8 10
3  6  9 12 15
4  8 12 16 20
5 10 15 20 25
```

Hint: You can use %2d in your printf functions to force all number displays to be 2 characters long (C will pad a space if the number is less than two digits)

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
int main(){
	int i, j,n;
	scanf("%d", &n);
	for(i = 1; i<=n;i++){
		for(j = 1; j<=n;j++){
			printf("%2d ", i * j);
		}
		printf("\n");
	}
	return 0;
}
```

</details>
