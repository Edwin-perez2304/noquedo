//Hacer un que realize la serie fibonacci -> 1+1+2+3+5+8+13...n  

#include<iostream>
#include<stdlib.h>
using namespace std;

int main(){
	int n,E=0,C=1,z=1;
	
	do{
		cout<<"Digite la cantidad de digitos de la serie: ";
		cin>>n;
	}while(n<=0);
	
	cout<<"1 <-> ";
	for(int i=1;i<n;i++){
		z = E + C;
		cout<<z<<" <-> ";
		E = C;
		C = z;		
	}
	
	cout<<"\n";
	system("pause");
	return 0;
}
