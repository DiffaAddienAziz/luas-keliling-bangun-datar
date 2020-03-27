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
  
int main(){
  	int sisi[2];
  	
  	for(int i=1 ; i<=2; i++){
  			sisi[2]=0;
  			
	  cout<<" Masukkan sisi persegi ke "<<i<<" : ";
	  cin>>sisi[i];
	  }
	  cout<<endl;
	  for(int i=1 ; i<=2 ; i++){
	  
	  cetak_luas(sisi[i]);
	  }
	  cout<<endl;
	  for (int i=1 ; i<=2 ; i++){
    	
    	cetak_keliling(sisi[i]);
    }
    return 0;
    }
