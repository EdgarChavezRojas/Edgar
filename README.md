/*
Edgar Chavez Rojas

Resolucion de formula cuadratica

*/
#include <iostream>
#include <cmath>
using namespace std;

int main()
{
    string resp; resp = "Si";
    float a, b ,c, d;
    while(resp == "Si" or resp == "si"){
    a=0; b=0; c=0; d = 0;
    cout<<"Digite el valor de a: "; cin>>a;
     cout<<"Digite el valor de b: "; cin>>b;
      cout<<"Digite el valor de c: "; cin>>c;
    
    d = b*b - 4*a*c;
    cout<<d;
    if( d > 0){
    cout<<"Las respuestas son: "<<endl;
    cout<< (-b-sqrt(d))/(2*a)<<endl;
    cout<< (-b+sqrt(d))/(2*a)<<endl;    
    }
    if(d == 0){
    cout<<"La respuesta unica es: "<<endl;
    cout<< (-b-sqrt(d))/(2*a)<<endl;
    }
    if(d < 0){
    cout<<"La solucion imaginaria es: "<<endl;
    cout<< (-b-sqrt(d*(-1)))/(2*a)<<"i"<<endl;
    cout<< (-b+sqrt(d*(-1)))/(2*a)<<"i"<<endl;    
    }
    
    cout<<"Desea hacer otros calculos?(Si/No): "; cin>>resp;
    } 
    return 0;
}
