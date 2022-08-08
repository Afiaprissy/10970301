// Agboado Priscilla Akorfa


// Student ID: 10970301

#include<iostream> 
using namespace std; 
  
bool isPrime(int n); 
  
int main() 
{   
  int num, sum=0, count=0; 
     
     cout<<"Kindly enter number: "; 
     cin>>num; 
      
  for(int j=0; count<num; j++) 
  { 
    if(isPrime(j))  
    { 
      sum += j; 
      count++;   
    } 
  } 
   
  cout<<"The average of the first "<<num<<" prime numbers is "<<(float)sum/count; 
} 
  
bool isPrime(int n) 
{ 
  bool frim = true; 
   
  if (n<2)    frim = false; 
  else if(n==2)  frim = true; 
  else 
  { 
    for(int i=2; i<=n/2; i++) 
    { 
      if(n%i==0) 
      { 
        frim = false; 
        break; 
      } 
    } 
  }   
  return frim;   
}
