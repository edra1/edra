#include <iostream>
using namespace std;
int main(){
         int opcion;
		 cout<<"1) Calcular Numeros Primos"<<endl;
		 cout<<"2) Factorial"<<endl;
		 cout<<"3) Calcular Promedio"<<endl;
		 cout<<"0) Salir"<<endl;
		 cout<<"Que opcion desea? ";
		 cin>>opcion;


		if (opcion==1)
		{

			 int cont=0,i,num;
        	 cout<<"Ingrese numero:";
         	cin>>num;
         	for(i=1;i<(num+1);i++)
		 	{
        		 if(num%i==0)
			 	{
        	     	cont++;
        		}

        	}
       			 if(cont!=2)
				 {
    	          cout<<"No es Primo";
    	    	 }
				 else
				 {
                cout<<"Si es Primo";
       	 	 	}
        }
        if (opcion==2)
        {
        	int num,res;
        	res=1;
        	cout<<"Dame un Numero:";
        	cin>>num;

        	for(int i=1;i<=num;i++)
        	{
        		res*=i;
			}
        	cout<<"EL FACTORIAL DE "<<num<<" ES: "<<res;
		}

		if (opcion==3)
		{
		    int num1,i,sum;
		    float prom;
		    i=0;
			do
            {
						
                cout<<"Dame un Numero:";
                cin>>num1;
                sum+=num1;
                i++;
                
            }while(num1!=(-1));
            prom=sum/(i-1.00);
            cout<<"Tu Promedio Es:"<<prom;
		}

		if (opcion==0)
		{
			cout<<"Adios :v";
		}
    return 0;
}
