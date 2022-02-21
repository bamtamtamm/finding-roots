# finding-roots
#include <iostream>
using namespace std;


int main()
{
    cout.setf(ios::fixed);
    cout.setf(ios::showpoint);
    cout.precision(16);
    
    long n,i=0,sign=1;
    double sum=0;
    
    cout<<"enter the number of terms:";
    cin>>n;
    
    do
    { i++;
    sum+=sign/(double)(2*i-1);
    sign*=-1;
}
while(i<=n);
cout<<"pi="<<4*sum<<endl;

return 0;

}
