#include<iostream>
#include<conio.h>

using namespace std;
main(){
	int op;
	float n1, n2, r;
	char c;
	cout<<endl<<"CALCULADORA BASICA";
	do{
		n1=0; n2=0; r=0;
	cout<<endl<<"1)Suma"<<endl<<"2)Resta"<<endl<<"3)Division"<<endl<<"4)Multiplicacion";
	cout<<endl<<"Selecciona una operacion a realizar: ";
	cin>>op;
	cout<<endl<<"Numero 1: ";
	cin>>n1;
	cout<<endl<<"Numero 2: ";
	cin>>n2;
	
	switch(op){
		case 1:
			r=n1+n2;
			cout<<endl<<"El  resultado es:"<<r;
			break;
		case 2:
			r=n1-n2;
			cout<<endl<<"El  resultado es:"<<r;
			break;
		case 3:
			if(n2==0){
				cout<<endl<<"No se puede dividir entre 0";
			}else{
				r=n1/n2;
				cout<<endl<<"El  resultado es:"<<r;
			}
			break;
		case 4:
			r=n1*n2;
			cout<<endl<<"El  resultado es:"<<r;
			break;
		default:
			cout<<endl<<"Vuelve a seleccionar un valor valido";
	}
	
	cout<<endl<<"¿Desea realizar otra operacion? s/n  ";
	cin>>c;
	}while(c=='s');
}
