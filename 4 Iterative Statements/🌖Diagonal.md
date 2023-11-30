# Diagonal Problem
Display an n diagonal line

For example, if n = 6, display:
```
*
 *
  *
   *
    *
     *
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
			if(i==j)
				printf("*");
			else
				printf(" ");
		printf("\n");		
	}
	return 0;
}
```
</details>