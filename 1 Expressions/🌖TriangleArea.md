# Triangle Area

Write a program that solves for the area of a triangle given its base and height user input

Area of triangle is 1/2 * base * height

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
	float base, height, bh, area;
	scanf("%f", &base);
	scanf("%f", &height);
	bh = base * height;
	area = bh * 1 / 2;
	printf("Area %f", area);
	return 0;
}
```

</details>
