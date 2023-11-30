# Cosine Similarity Problem
Write a function that computes for the cosine similarity of 2 a float variable to 2 b float variable user inputs

![Cosine Similarity Formula](https://miro.medium.com/v2/resize:fit:720/format:webp/1*LfW66-WsYkFqWc4XYJbEJg.png "Cosine Similarity Formula")


<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
#include<math.h>

float
cosineSimilarity(float a1, float a2, float b1, float b2){
	float numerator, denominator, cosine;
	numerator = a1*b1+a2*b2;
	denominator = sqrt(a1*a1 + a2*a2) * sqrt(b1*b1 + b2*b2);
	cosine = numerator / denominator;
	return cosine;
}
```

</details>
