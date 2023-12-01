# Convert to binary
Write a program that reverses the digits of a 3 digit integer

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
	int a, dig1, dig2, dig3, reverse;
	a = 123;
	dig1 = a / 100;
	dig2 = a / 10 % 10;
	dig3 = a % 10;
	reverse = dig3 * 100 + dig2 * 10 + dig1;
	printf("%d", reverse);
	return 0;
}
```

</details>
