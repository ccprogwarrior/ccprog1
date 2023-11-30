# Cosine Similarity Problem
Write a function that computes for the cosine similarity of 2 x float variable to 2 y float variable user inputs

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
cosineSimilarity(float x1, float x2, float y1, float y2){
	float numerator, denominator, cosine;
	numerator = x1*y1+x2*y2;
	denominator = sqrt(x1*x1 + x2*x2) * sqrt(y1*y1 + y2*y2);
	cosine = numerator / denominator;
	return cosine;
}
```

</details>
