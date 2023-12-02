# Division Algorithm Problem
In Elementary Number Theory (a field in mathematics that deals with the study of integers), there's a theorem called Division Algorithm. which states that given an integer n and d (divisor), there exists a unique combination of integers q  (quotient) and r (remainder) such that 0 <= r < d and

n = dq + r

Note that according to the Division Algorithm theorem, the value of r cannot be negative.

Example 1: if n = 30 and d = 4, then q = 7 and r = 2

Example 2: if n = 21 and d = 3, then q = 7 and r = 0

Example 3: if n = -10 and d = 7, then q = -2 and r = 4

Example 4: if n = -5 and d = -2, then q = 3 and r = 1

Example 5: if n = 3 and d = 5, then q = 0 and r = 3

Create a program that contains a function that derives the values of q (quotient) and r (remainder) given user inputted values for n (integer) and d (divisor). You may assume that the user will never input 0 as value for divisor.

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
void getRemainderQuotient(int nInt, int nDiv, int* nRemainder, int* nQuotient){
	*nQuotient = nInt / nDiv;
	if(nInt - (*nQuotient) * nDiv < 0){
		(*nQuotient) += 1;
	}
	if(nInt < 0 && nDiv > 0){
		(*nQuotient) *= -1;
	}
	*nRemainder = nInt - (*nQuotient) * nDiv;
}
```

</details>
