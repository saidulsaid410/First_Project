# First_Project
#include<bits/stdc++.h>
#include<windows.h>
using namespace std;
int main(){
    int h,m,s,a,err;
    err=0;
    while (err==0)
    {   
        cout<<"\nEnter Hour: ";
        cin>>h;
         cout<<"Enter Minutes: ";
         cin>>m;
          cout<<"Enter Secont: ";
          cin>>s;
          if( h<=24 && m<60 && s<60 )
          err++;
          if(h>24 || m>60 || s>60)
          cout<<"Time does not Exist";
          else
          system("cls");     
    }
    while(true){
        system("cls");
        cout<<h<<":"<<m<<":"<<s<<endl;
        Sleep(1000);
        s++;
        if(s>59)
        {
            s=0;
            m++;
        }
        if(m>59)
        {
            m=0;
            h++;
        }
        if(h>=24)
        {
            h=0;
        }  
    }
      return 0;
}
