#include<iostream>
using namespace std;

//do while loop
int sum(int n)
{
    int sum=0;
    do
    {
        sum=sum+n;
        n--;

    }while(n>0);

    return sum;
}

//for loop
int sum(int n)
{
    int sum = 0;
    for(int i=n; i>0; i--)
    {
        sum=sum+i;
    }

    return sum;
}

//recursive function
int sum(int n)
{

    if (n==1)
    {
        return 1;
    }
    else
    {
        return n+sum(n-1);
    }
}

//no loop & no recursion
int sum(int n)
{
    int sum=0;
    sum=n*(n+1)/2;
}

int main()
{
    cout<<"There are many ways of doing the function to get sum of the terms..."<<endl;
    cout<<sum(4);

    return 0;
}
