# Adding Time Problem
Create a C program that accepts 2 military time, represented as 4-digit integers, and adds them.

Military time ranges from 0000 to 2359.

time1=1300 and time2=200
output
```
1500 same day
```

time1=2359 and time2=1
output
```
0 next day
```

time1=930 and time2=1030
output
```
2000 same day
```

<details>
<summary>Explanation</summary>
<br>
</details>


<details>
<summary>Answer</summary>
<br>

``` c
int main(){
	int time1, time2, hh1, mm1, hh2, mm2, mm, hh, time, nextDay;
	scanf("%d", &time1);
	scanf("%d", &time2);
	nextDay = 0;
	hh1=time1/100;
	hh2=time2/100;
	mm1=time1%100;
	mm2=time2%100;
	hh=hh1+hh2;
	mm=mm1+mm2;
	if(mm>=60)
	{
	hh=hh+1;
		mm=mm-60;
	}
	if(hh>23)
	{
		hh=hh-23;
		nextDay=1;
	}
	time=hh*100+mm;
	if(nextDay==1)
		printf("%d Next Day", time);
	else
		printf("%d Same Day", time);
	return 0;
}
```
</details>