#include<bits/stdc++.h>
using namespace std;
bool my_comp(int a,int b){
  string z=to_string(a);
  string x=to_string(b);
  int q=0,w=0;
  for(int i=0;i<z.length();i++){
    q=q+(z[i]-48);
  }
    for(int i=0;i<x.length();i++){
    w=w+(x[i]-48);
  }
  if(q<w)
  return true;
  else
  return false;
}
int main() {

int n;
cin>>n;


vector<int> v;
for(int i=1;i<=n;i++){
  v.push_back(i*2);

}
for(auto i=v.begin();i!=v.end();i++){
cout<<*i;
if(i!=v.end()-1)
cout<<" ";}

cout<<endl;
sort(v.rbegin(),v.rend());
for(auto i=v.begin();i!=v.end();i++){
cout<<*i;
if(i!=v.end()-1)
cout<<" ";}
cout<<endl;
reverse(v.begin(),v.end());
for(auto i=v.begin();i!=v.end();i++){
cout<<*i;
if(i!=v.end()-1)
cout<<" ";}
unordered_set <int> s;
for(auto i=v.begin();i!=v.end();i++)
s.insert(*i);
cout<<endl;
cout<<*lower_bound(v.begin(),v.end(),1000)-1;
sort(v.begin(),v.end(),my_comp);
cout<<endl;
for(auto i=v.begin();i!=v.end();i++){
cout<<*i;
if(i!=v.end()-1)
cout<<" ";}
cout<<endl;
//sort(v.begin(),v.end());

map<int,int>mp;
for(int i=0;i<v.size();i++){
  mp[i]=*s.find(v[i]);
}

for(int i=0;i<v.size();i++){
cout<<(i+1)*2<<":"<<v[i];
if(i!=v.size()-1)
cout<<" ";
}

  return 0;
}
