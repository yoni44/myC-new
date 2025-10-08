#include <iostream>
#include<cmath>
using namespace std;

int main() {
	int year;
	cout<<"Enter Year:";

	cin>> year;
	int a = year % 19;
	int b = year % 4;
	int c = year % 7;
	int d = (a*19+24)%30;
	int e = (2*b + 4*c + 6*d + 5)%7;
	if(d+e < 10)
	{
		cout<<"Easter falls on March "<< d+e+22;
	}
	else
	{
		cout<<"Easter falls on April "<< d+e-9;
	}
	return 0;
}
