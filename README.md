# palindrome-0.0.1

#include "stdafx.h"
#include "iostream"
#include "string"

using namespace std;


int main()
{
	string a, b;
	char n;
	int i, j;

	cin >>a ;

	b = a;

	for (i = 0, j = a.length() - 1; j > i; i++, j--) {
		n = a[i];
		a[i] = a[j];
		a[j] = n;
	}

	if (a == b) cout << "1" << endl;
	else cout << "0" << endl;
	
	system("pause");
	return 0;
}
