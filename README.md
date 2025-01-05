# Car-parking-project
#include<iostream>
using namespace std;

int main(){
    int r=0;
    int c=0;
    int b=0;

    int u_input;

    int amount=0,count=0;
    //menu
    while(true){


    cout<<"Press 1 for rickshaw"<<endl;
    cout<<"Press 2 for car"<<endl;
    cout<<"Press 3 for bus"<<endl;
    cout<<"Press 4 to show the record"<<endl;
    cout<<"Press 5 to deleted records"<<endl;
    cin>>u_input;

    if(u_input==1){
        r++;
        if(count<=50){
        amount=amount+100;
        count=count+1;
        }else{
            cout<<"no parking"<<endl;
        }
    }else if(u_input==2){
        c++;
        if(count<=50){
        amount=amount+200;
        count=count+2;
        }else{
            cout<<"no parking"<<endl;
        }
    }else if(u_input==3){
        b++;
        if (count<=50){
        amount=amount+300;
        count=count+3;
        }else{
            cout<<"no parking"<<endl;
        }
    }else if(u_input==4){
        cout<<"*************************************************"<<endl;
        cout<<"total amount collected="<<amount<<endl;
        cout<<"total car parked="<<count<<endl;
        cout<<"number of rickshaw parked="<<r<<endl;
        cout<<"number of car parked="<<c<<endl;
        cout<<"number of bus parked="<<b<<endl;
        cout<<"*************************************************"<<endl;
    }else if(u_input==5){
        amount=0;
        count=0;
        cout<<"all records deleted"<<endl;
        r=0;
        c=0;
        b=0;
        cout<<"*********************************"<<endl;
        cout<<"DELETED RECORD"<<endl;
        cout<<"*********************************"<<endl;
    }else{
        cout<<"invalid number"<<endl;
    }

    }
        








    return 0;
}
