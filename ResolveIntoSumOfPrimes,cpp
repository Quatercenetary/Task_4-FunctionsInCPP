#include <iostream>

using namespace std;

bool PrimeOrNot(int a){
    for(int i = 2; i <= a/2; i++){ // a/2 because values between a and a/2 result in decimals less than 1. 
        if(a % i == 0){
            return 0;
        }
    }
    return 1;
}

int main(){
    int x, y = 0;
    cout<<"Enter a number: ";
    cin>> x;
    for(int i = 2; i <= x/2; i++){
        if(PrimeOrNot(i)){ //Checking if number is prime
            if(PrimeOrNot(x-i)){ //Checking if complemetary number is prime 
                cout<<x<<" = "<<i<<" + "<<x-i<<endl; //If both are prime, then display
                y++;
            }
        }
    }
    if(y == 0) cout<<"Can not express this number as sum of two prime numbers."; //for example, 3

    return 0;
}
