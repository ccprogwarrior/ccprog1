# XOR
Create a function that simulates the XOR operator

XOR truth table

1 xor 1 = 0
1 xor 0 = 1
0 xor 1 = 1
0 xor 0 = 0

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
int 
xorfunction(int a, int b){
	return a != b && (a || b);
}
```
</details>