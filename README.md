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
O/P: ![image](https://github.com/user-attachments/assets/76b7a341-579f-42d6-bc8c-d066cda5b992)





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
O/P: ![image](https://github.com/user-attachments/assets/6056ac24-7df2-4448-9173-cea5f01e55ee)




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
O/P:  ![image](https://github.com/user-attachments/assets/cca760b8-c0ca-4253-a0bd-f5367ead4a41)



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
O/P:  ![image](https://github.com/user-attachments/assets/bac20ec1-803c-4241-b750-6b4d7a0372f2)


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
O/P: ![image](https://github.com/user-attachments/assets/acbf5579-c6fa-47a7-ba71-78f236b4fb89)




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
O/P: ![image](https://github.com/user-attachments/assets/84daaae9-deb6-40e0-b3aa-78c552af5857)


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
O/P: ![image](https://github.com/user-attachments/assets/23e1e9bd-a34e-49fd-abf4-751c0bb7d694)



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
O/P: ![image](https://github.com/user-attachments/assets/c9954e2d-12e8-41e7-b657-0b9526ca11f6)




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
O/P: ![image](https://github.com/user-attachments/assets/8bcc5364-2e9f-45f2-b849-034bbcf04891)




CONCLUSION:

In this experiment we used the different loops and their nested combinations, which are essential for programming and managing complex iterations. For loops are ideal for known iterations, whileloops for condition basis and do while for executing the code at least once.

Nested loops are used for more complex tasks, and understanding them is effective in handling those tasks.
