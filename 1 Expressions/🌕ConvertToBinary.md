# Convert to binary
Write a program that converts a 2 digit integer to binary

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
	int a, binary;
	
	a = 99;
	binary = a / 64 * 10;
	a = a - a / 64 * 64;
	
	binary = (binary + a / 32) * 10;
	a = a - a / 32 * 32;
	
	binary = (binary + a / 16) * 10;
	a = a - a / 16 * 16;
	
	binary = (binary + a / 8) * 10;
	a = a - a / 8 * 8;
	
	binary = (binary + a / 4) * 10;
	a = a - a / 4 * 4;
	
	binary = (binary + a / 2) * 10;
	a = a - a / 2 * 2;
	
	binary = binary + a;
	
	printf("%d", binary);
	
	return 0;
}
```
[Run it on Replit](https://replit.com/@ccproglearner/ccprog1replit#expressions-Converttobinary1.c)
</details>


<details>
<summary>Answer 2</summary>
<br>

``` c
#include<stdio.h>
int 
main(){
int a, binary;
a = 99;
binary = a / 64 * 10;
a = a % 64;
binary = (binary + a / 32) * 10;
a = a %32;
binary = (binary + a / 16) * 10;
a = a%16;
binary = (binary + a / 8) * 10;
a = a % 8;
binary = (binary + a / 4) * 10;
a = a%4;
binary = (binary + a / 2) * 10;
a = a %2;
binary = binary + a;
printf("%d", binary);
return 0;
}
```
[Run it on Replit](https://replit.com/@ccproglearner/ccprog1replit#expressions-Converttobinary2.c)
</details>
