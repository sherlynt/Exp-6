# Experiment-6

AIM: To study and implement C++ decision making statements loops.

SOFTWARE: Visual Studio Code

THEORY: 
Loops are a fundamental part of programming which allow a block of code to iterate on basis of some given conditions. The types of loops are:

1] For loop: 
It is used when we know how many times we want a block of code to be executed. It consists of three parts- initialization, condition, increment/ decrement.

2] While loops:
While loop is used when we do not know how many times we want the block of code to executed. It continues to be executed as long as the given condition holds to be true. The condition is checked before the code is executed.

3] Do While loop:
It is similar to the while loop, but it checks the condition after the code is executed. Hence the code is executed at least once.

4]Nested Loops:
Nested loops are loops inside a loop. They are used in multidimensional arrays or creating patterns.

CODE:

For loop

```
#include<iostream>
using namespace std;
int main(){
    int i;
    for(i=0;i<20;i++){
        cout<<i<<endl;
    }
}
```
O/P: ![image](https://github.com/user-attachments/assets/c1e5aff8-e61d-49de-872c-9b5c2fe2c31b)




While Loop

```
#include<iostream>
using namespace std;
int main(){
    int i=0;
    while(i<10){
        cout<<i<<endl;
        i++;
    }
}
```
O/P: ![image](https://github.com/user-attachments/assets/88f1e538-289a-4f89-b105-c9e441162cb7)



Do While Loop
```
#include<iostream>
using namespace std;
int main(){
    int i=0;
    do{
        cout<<i<<endl;
        i++;
    }
        while(i<10);
        return 0;     
}
```
O/P: ![image](https://github.com/user-attachments/assets/62d56b2f-9716-455c-a444-3e053b26d14e)




Nested For 
```
#include <iostream>
using namespace std;

int main() {
    for (int i=1; i<=10; i++) {
        for (int j=1;j<=10;j++) {
            cout <<i*j<<"\t"; 
        }
        cout << endl;
    }
    return 0;
}
```
O/P: ![image](https://github.com/user-attachments/assets/5d03c011-cc8b-4706-be34-389efcfb7ade)




Nested While
```
#include <iostream>
using namespace std;

int main() {
    int i=1;
    while (i<=10) {
        int j=1;  
        while (j<=10) {
            cout<<i*j<<"\t"; 
            j++;
        }
        cout<<endl; 
        i++;
    }
    return 0;
}
```
O/P: ![image](https://github.com/user-attachments/assets/e4b5d767-6f14-491f-a6bf-1f9d36902dc3)




Nested Do While
```
#include <iostream>
using namespace std;

int main() {
    int i = 1;
    do {
        int j=1;
        do {
            cout<<i * j<< "\t"; 
            j++;
        } while (j<=10);
        cout<<endl; 
        i++;
    } while (i<=10);
    return 0;
}
```
O/P: ![image](https://github.com/user-attachments/assets/9cadbff7-4d0d-4a0e-8433-1960d942444e)




For loop inside while loop:
```
#include <iostream>
using namespace std;
int main() {
    int i=1;
    while (i<=5) {
        for (int j=1; j<=5; j++) {
            cout << i*j <<"\t"; 
        }
        cout << endl; 
        i++;
    }
    return 0;
}
```
O/P: ![image](https://github.com/user-attachments/assets/e547583c-bd23-497b-a869-3a44ce2cbb27)


While loop inside for loop:
```
#include <iostream>
using namespace std;

int main() {
    
    for (int i=1; i<=5; i++) {
        int j=1;

        while (j <= i) {
            cout << "* ";
            j++;
        }
        cout << endl; 
    }
    return 0;
}
```
O/P: ![image](https://github.com/user-attachments/assets/abef47fd-7c09-4ab0-8783-59ec499c33df)



```
#include<iostream>
using namespace std;
int main(){
    int i,j,k=0,n;
    cout<<"Enter number of rows:";
    cin>>n;
    for(i=1;i<=n;i++){
        for(j=1;j<=(n-i);j++){
        cout<<"  ";
    }
    while(k!=(2*i-1)){
        cout<<"* ";
        k++;
    }
    k=0;
    cout<<endl;
}
cout<<endl;
    }
```
O/P: ![image](https://github.com/user-attachments/assets/ac96cf39-0df4-4ee5-89d2-e03aba68b768)



CONCLUSION:

In this experiment we used the different loops and their nested combinations, which are essential for programming and managing complex iterations. For loops are ideal for known iterations, whileloops for condition basis and do while for executing the code at least once.

Nested loops are used for more complex tasks, and understanding them is effective in handling those tasks.
