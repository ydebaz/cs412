#include <iostream>
#include<string>
#include<algorithm>
using namespace std;


int binaryToDecimal(int n) 
{ 
    int num = n; 
    int dec_value = 0; 
  
    // Initializing base value to 1, i.e 2^0 
    int base = 1; 
  
    int temp = num; 
    while (temp) { 
        int last_digit = temp % 10; 
        temp = temp / 10; 
  
        dec_value += last_digit * base; 
  
        base = base * 2; 
    } 
  
    return dec_value; 
}
int main() {
  const int s1[4][16] =
	{ /* S1 */
		14,4,13,1,2,15,11,8,3,10,6,12,5,9,0,7,
		0,15,7,4,14,2,13,1,10,6,12,11,9,5,3,8,
		4,1,14,8,13,6,2,11,15,12,9,7,3,10,5,0,
		15,12,8,2,4,9,1,7,5,11,3,14,10,0,6,13
	};
  int n,a[6];
  //get the number
  cin>>n;
 
  for(int i=0; n>0; i++)    
{    
a[i]=n%2;    
n= n/2;  
} 

reverse(a,a+6);
//turn to binary
for(int i=0;i<6;i++){cout<<a[i];}

cout<<endl;
char ss[2];
ss[0]=((char)(a[0]+48));
ss[1]=((char)(a[5]+48));

char se[4];
se[0]=((char)(a[1]+48));
se[1]=((char)(a[2]+48));
se[2]=((char)(a[3]+48));
se[3]=((char)(a[4]+48));

string q=string(ss);
string w=string(se);
w.pop_back();
w.pop_back();
w.pop_back();

cout<<q<<" "<<w<<endl;

//take the 2 numbers in binary
int z=std::atoi(q.c_str());
int x=std::atoi(w.c_str());
//change from binary to decimal 
int c=binaryToDecimal(z);
int v=binaryToDecimal(x);
cout<<c<<" "<<v<<endl;
//find the number in s1
cout<<s1[c][v];
}
