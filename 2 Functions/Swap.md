# Swap Value Problem 🌖
Write a function that swaps the values of 2 integers using pointers


<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
void 
swap(int * val1, int * val2){
	int temp = *val1;
	*val1 = *val2;
	*val2 = temp;
}
```

</details>
