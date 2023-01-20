//Bubble sort using C++//
#include<iostream>
using namespace std;


void mySort(int array[], int n){
    for(int i=0; i<n; i++){
        for(int j=i + 1; j<n; j++){
            if(array[i] > array[j]){
                int temp = array[i];
                array[i] = array[j];
                array[j] = temp;
            }
        }
    }
}

void p(int array[], int n){
    for(int i=0; i<n; i++){
        cout<<" "<<array[i];
    }
    cout<<endl;
}

int main(){
    int array[] = {8,7,4,6,11,77,2,1,55};
    int n = 9;
    
    mySort(array, n);
    p(array, n);
}
