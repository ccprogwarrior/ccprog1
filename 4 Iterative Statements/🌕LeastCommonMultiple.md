# Least Common Multiple Problem
Write a function that gets the least common multiple of 2 integers

lcm(10, 5) returns 10

lcm(3, 2) returns 6

lcm(100, 111) returns 11100

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
int lcm(int a, int b){
	int i = 1, j = 1;
	while(a*i != b*j){
		if(a*i < b*j)
			i++;
		else if (b*j < a*i)
			j++;
	}
	return a*i;
}
```

</details>
