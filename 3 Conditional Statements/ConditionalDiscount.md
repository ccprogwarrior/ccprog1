# Box Border Problem
A retail store issued a promo that gives a 30% discount on all items, so long as the final price remains above 100. Write a program that computes for the final price of
an item.

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
int main(){
	float price;
	printf("price of item: ");
	scanf("%f", &price);

	if(price - (price * 0.3) > 100)
		price = price - (price * 0.3);
		
	printf("final price of item is: %.2f", price);
	
	return 0;
}
```
</details>

