# Box Border Problem
Display the borders of an n x n box of asterisks.

For example, if n = 6, display:
```
******
*    *
*    *
*    *
*    *
******
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
	int i, j,n;
	scanf("%d", &n);
	for(i=0;i<n; i++){
		for(j=0; j<n;j++)
			if(i==0||j==0||i==n-1||j==n-1)
				printf("*");
			else
				printf(" ");
		printf("\n");		
	}
	return 0;
}
```
</details>
