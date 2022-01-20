# MINFD_codeChef
#include <bits/stdc++.h>
using namespace std;
int main() {
	int t;
	cin>>t;
	while(t--){
	    int ar[100]={0};
	    int n,a;
	    cin>>n>>a;
	    for(int i=0;i<n;i++){
	        cin>>ar[i];
	    }
	    sort(ar, ar + n, greater<int>());
	    bool f=false;
	    int sum=0;
	    for(int j=0;j<n;j++){
	        sum=sum+ar[j];
	        if(sum>=a){
	            
	            cout<<j+1<<endl;
	            f=true;
	            break;
	        }
	    }if(f==false)cout<<"-1\n";
	}
	return 0;
}
