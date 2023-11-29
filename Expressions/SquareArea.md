# Square Area
Write a program that solves for the area of a square given its side length

Area of square = side * side

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
#include<stdio.h>
float squareArea(float side){
	float area;
	area = side * side;
	return area;
}

int main(){
	float side;
	scanf("%f", &side);
	printf("Area %f", squareArea(base, height));
	return 0;
}
```

</details>