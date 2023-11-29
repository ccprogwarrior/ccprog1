# Triangle Area
Write a program that solves for the area of a triangle given its base and height.

Area of triangle is 1/2 base * height

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
#include<stdio.h>
float triangleArea(float base, float height){
	float bh, area;
	bh = base * height;
	area = bh * 1 / 2;
	return area;
}

int main(){
	float base, height;
	scanf("%f", &base);
	scanf("%f", &height);
	printf("Area %f", triangleArea(base, height));
	return 0;
}
```

</details>