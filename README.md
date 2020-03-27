// luas-keliling-persegi
// implementasi pointer array dan fungsi 


#include <iostream>
#include <cmath>
using namespace std;
  
  
  int luas_persegi(int sisi){
  	int luas;
	  luas = 0;
	  luas = sisi * sisi;
	  return luas;
  }
  
  int keliling_persegi(int sisi){
  	int keliling ;
	  keliling = 0;
	  keliling = sisi * 4;
	  return keliling;
  }
  
  void cetak_luas(int s){
  	
  	  cout<<"Luas persegi adalah : "<<luas_persegi(s)<<endl;
     }
  
  void cetak_keliling(int s){
  	
	  cout<<"Keliling persegi adalah : "<<keliling_persegi(s)<<endl;
  }
  const int MAX = 3;
int main(){
  	int sisi[MAX];
  	int *ptr[MAX];
  	
  	for(int i=2 ; i<=MAX; i++){
  			ptr[i] = &sisi[i]; 
  			
	  cout<<" masukkan sisi persegi ke "<<i-1<<" : ";
	  cin>>*ptr[i];
	  }
	  cout<<endl;
	  for(int i=2 ; i<=MAX ; i++){
	  
	  cetak_luas(*ptr[i]);
	  }
	  cout<<endl;
	  for (int i=2 ; i<=MAX ; i++){
    	
    	cetak_keliling(*ptr[i]);
    }
    return 0;
    }
