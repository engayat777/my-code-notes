/******************************************************************************

                              Online C++ Compiler.
               Code, Compile, Run and Debug C++ program online.
Write your code in this editor and press "Run" button to compile and execute it.

*******************************************************************************/

#include <iostream>
using namespace std;

int main()
{
int size=5;
int element=0;
int index=0;
int arr[size]={10,20,30,40,50};

cout<<" Array before editing : ";
for(int i=0;i<size;i++)
{
    cout<<arr[i]<<" ";
}
cout<<endl;
cout<<" enter element that you want to insert :";
cin>>element;

cout<<"enter index : ";
cin>>index;

if(index>size)
{
    cout<< "invalid index "<<endl;
}
else
{
    for(int i=size;i>index;i--)
    {
        arr[i]=arr[i-1];
    }
    arr[index]=element;
size++;
}
cout<<endl;
cout<<" Array after editing : ";
for(int i=0;i<size;i++)
{
    cout<<arr[i]<<" ";
}
cout<<endl;
    return 0;
}
