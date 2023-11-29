# Integer to Raised Problem
Write a function that computes for the raised value of an integer


<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
int raise(int x, int raise){
	int i, res;
	res = 1;
	for(i = 0; i < raise; i++){
		res *= x;
	}
	return res;
}
```

</details>