# Zodiac Sign Problem
Given a month and day input, determine the zodiac sign of the date.

Aries ♈️: March 21 - April 19

Taurus ♉️: April 20 - May 20

Gemini ♊️: May 21 - June 20

Cancer ♋️: June 21 - July 22

Leo ♌️: July 23 - August 22

Virgo ♍️: August 23 - September 22

Libra ♎️: September 23 - October 22

Scorpio ♏️: October 23 - November 21

Sagittarius ♐️: November 22 - December 21

Capricorn ♑️: December 22 - January 19

Aquarius ♒️: January 20 - February 18

Pisces ♓️: February 19 - March 20

Assume that the month and day inputs are valid.

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
	int day, month;
	
	printf("Month: "); scanf("%d", &month);
	printf("Day: "); scanf("%d", &day);
	
	
	switch(month){
		case 3:
			if (day <= 21) printf("Aries");
			else printf("Pisces");
			break;
		case 4:
			if(day <= 19) printf("Aries");
			else printf("Taurus");
			break;
		case 5:
			if(day <= 21) printf("Taurus");
			else printf("Gemini");
			break;
		case 6:
			if(day <= 20) printf("Gemini");
			else printf("Cancer");
			break;
		case 7:
			if(day <= 22) printf("Cancer");
			else printf("Leo");
			break;
		case 8:
			if(day<=22) printf("Leo");
			else printf("Virgo");
			break;
		case 9:
			if(day<=22) printf("Virgo");
			else printf("Libra");
			break;
		case 10:
			if(day<=22) printf("Libra");
			else printf("Scorpio");
			break;
		case 11:
			if(day <= 21) printf("Scorpio");
			else printf("Sagittarius");
			break;
		case 12:
			if(day <= 21) printf("Saggitarius");
			else printf("Capricorn");
			break;
		case 1:
			if(day <19) printf("Capricorn");
			else printf("Aquarius");
			break;
		case 2:
			if(day <= 18) printf("Aquarius");
			else printf("Pisces");
			break;
	}
	
	return 0;
}
```
</details>