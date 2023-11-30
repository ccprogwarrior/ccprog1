# Celsius to Fahrenheit Problem (Difficulty: 🌗)
Write a program that converts a temperature from degrees Celsius to degrees Fahrenheit.

Note that C = 5/9 (F - 32)

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
	float celsius, fahrenheit;
	printf("celsius: ");
	scanf("%f", &celsius);
	fahrenheit = 9.0 / 5 * celsius + 32;
	printf("fahrenheit %f", fahrenheit);
	return 0;
}
```

</details>
