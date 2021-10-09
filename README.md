#include<iostream>
using namespace std;
class tollboth
{
unsigned int car;
double amt;
public:
tollboth()
{
this->car=0;
this->amt=0;
}
void playcar()
{
this->car++;
this->amt=50;
}
void nonplaycar()
{
this->car++;
}
void display()
{
cout<<"name of car"<<car<<endl;
cout<<"amount:"<<amt<<endl;
}
};
int main()
{
char c='y';
int ch;
tollboth t;
do
{
cout<<"1 for paying\n 2 for non playing\n 3 display/exit\n";
cout<<"enter choice\n";
cin>>ch;
switch(ch)
{
case 1:
t.playcar();
cout<<"car added";
break;
case 2:
t.nonplaycar();
cout<<"car added";
break;
case 3:
t.display();
c='n';
break;
}
if(c=='y'||c=='Y')
{
cout<<"\ndo you want to continue";
cin>>c;
}
}
while(c=='y'||c=='Y');
return 0;
}

