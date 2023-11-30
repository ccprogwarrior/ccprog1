# Copy Value Problem
Write a function that copies the value of an input integer to another integer variable.

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
void 
copy(int val1, int * val2){
	*val2 = val1;
}

int 
main(){
	int input, storehere;
	printf("input integer ");
	scanf("%d", &input);
	copy(input, &storehere);
	printf("storehere value: %d", storehere);
}
```

</details>

