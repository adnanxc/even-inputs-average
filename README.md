# even-inputs-average
Write a program that takes 5 inputs from the users and finds the average of even inputs only. If there is no even inputs from the user, it prints 0.


#include <iostream>
using namespace std;

int average(int m , int n , int o , int p , int q){
    int sum = 0;
    if (m % 2==0){
        sum+=m;
    }
    if (n%2==0){
        sum+=n;
    }
    if (o%2==0){
        sum+=o;
    }
    if (p%2==0){
        sum+=p;
    }
    if (q%2==0){
        sum+=q;
    }
    int av = sum/2;
    return av;
}

int main(){

    int a , b , c , d , e;
    cout << "Enter all 5 inputs (use tab to enter each input): ";
    cin >> a;
    cin >> b;
    cin >> c;
    cin >> d;
    cin >> e;
    int s = average(a , b , c , d , e);
    cout << "Average for even numbers: " << s;
    return 0;
}
