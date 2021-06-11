#include<iostream>
using namespace std;
void input(int* a, int n) {

	for (int i = 0; i < n; i++) {
		cin >> a[i];
	}
}
void output(int* a, int n) {
	for (int i = 0; i < n; i++) {
		cout << a[i]<<endl;
	}
}
int* findMax(int* a, int n) {
	int* max;
	max = &a[0];
	for (int i = 0; i < n; i++) {
		if (a[i] > * max) {
			max = &a[i];
		}
	}
	//cout << max;
	return max;
}
int main(){
	int n,*a;
	cin >> n;
	a = new int[n];
	input(a, n);
	cout << *findMax(a, n)<<endl;
	output(a, n);


}
Gobitech/Gobitech is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
