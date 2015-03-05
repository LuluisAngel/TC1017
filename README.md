# TC1017
CODES


    #include <iostream>
    #include <cmath>
    
    //Luis Angel Aguilar Carrillo A01225421
    
    using namespace std;
    
    float prom(float x){
    
    	return (x/10);
    }
    
    int main(){
    	
    	int sum=0;
    	float dif, var=0;
    	float numeros[10];
    
    	
    	for (int i=0; i<10; i++){
    	
    	cout << "Introduce un numero" << endl;
    	cin >> numeros[i];
    	
    	sum = sum + numeros[i];
    	}
    
    	for (int j=0; j<10; j++){
    
    		dif = (numeros[j])-prom(sum);
    		var = var + (pow(dif,2));
    	}
    
    	var = var / 10;
    	var = pow (var,(0.5));
    
    	cout << "La suma de todos los numeros es de " <<sum << endl;
    	cout << "El promedio de esos numeros es de " << prom(sum) << endl;
    	cout << "La desviación estandar de los numeros es " << var << endl;
    
    
    	return 0;
    }
