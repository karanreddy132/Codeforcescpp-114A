# Codeforcescpp-114A
#include <bits/stdc++.h>
using namespace std;

int main() {
	long long int n,l,k(1);
  cin >> n;
  cin >> l;
  if(l%n!=0){
    cout << "NO";
  }
  else{
    while(pow(n,k)!=l && pow(n,k)<l){
    k++;
    }
    if(pow(n,k)==l){
      cout << "YES" << endl << k-1;
    }
    else{
      cout << "NO";
    }
  }
	return 0;
}
