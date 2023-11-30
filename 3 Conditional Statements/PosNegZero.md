# Positive, Negative or Zero
Write a program that determines if an input is positive, negative or 0.

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
#include<stdio.h>
int main(){
	int input;
	if(input > 0){
		printf("Positive");
	} else if(input<0){
		printf("Negative");
	} else if(input==0){
		printf("Zero");
	}
	return 0;
}
```

</details>