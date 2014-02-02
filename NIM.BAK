#include<iostream.h>
#include<conio.h>
#include<process.h>
#include<iomanip.h>
#include<dos.h>
void selection();
void display();
void moving();
void ending();
void rules();
int *a;
char x='A';
char p1[20] , p2[20];
int turn = 0;
void main()
{
clrscr();
gotoxy(24,10);
cout<<"WELCOME TO THE NIM GAME MADE BY SAURABH "<<endl;
gotoxy(24,11);
cout<<"________________________________________"<<endl;
cin.get();
clrscr();
rules();
selection();

getch();
}
void rules()
{
cout<<" THIS GAME WILL HAVE 2 PLAYERS "<<endl;
cout<<" " <<endl;
cout<<" FIRST OF ALL PLZ ON YOUR CAPSLOCK KEY "   <<endl;
cout<<" "<<endl;
cout<<" IN THIS YOU HAVE TO TAKE OBJECTS FROM THE HEAP (A , B , C , D) TURN WISE "<<endl;
cout<<" "<<endl;
cout<<" THE PLAYER WHO TAKE OUT THE LAST OBJECT WILL BE THE WINNER OF THE GAME "<<endl;
cout<<" " <<endl;
cout<<" FOR THIS YOU HAVE TO FIRST INPUT THE NAME OF HEAP AND THAN NUMBER OF "<<endl;
cout<<"  ELEMENTS YOU WANT TO TAKE FROM THAT HEAP "<<endl;
cout<<" " << endl;
cout<<" ONE HEAP CAN TAKE MAXIMUM OF 9 OBJECTS SO INPUT THE NUMBER OF OBJECTS CAREFULLY"<<endl;
cout<<" BEFORE STARTING THE GAME "<<endl;
cout<< " "<<endl;
cout<<" YOU CAN PRESS 'E' FOR EXIT AT ANY TIME BETWEEN THE GAME " <<endl;
cout<<" "<<endl;
cout<<" PRESS ENTER TO PROCEED FURTHER "<<endl;
cin.get();
clrscr();
}
void selection()
{
int obj;
char y;
cout<<"ENTER THE NAME OF PLAYER 1 "<<endl;
cin.get(p1,15);
cout<<"ENTER THE NAME OF PLAYER 2 "<<endl;
cin>>p2;

a = new int[3];
cout<<"MAXIMUM NUMBER OF OBJECTS A HEAP CAN HAVE IS 9 "<<endl;
cout<<" "<<endl;
for(int i=0;i<3;i++)
{
 y = x+i;
	cout<<"ENTER THE OBJECTS IN HEAP "<<y<<endl;
	cin>>obj;
	a[i] = obj;
}
cin.get();
clrscr();
gotoxy(24,10);
cout<<p1<<" WILL START THE GAME "<<endl;
cout<<""<<endl;
gotoxy(24,11);
cout<<"BEST OF LUCK"<<endl;
cout<<""<<endl;
gotoxy(24,12);
cout<<"PRESS ENTER TO START THE GAME "<<endl;
cin.get();
clrscr();
display();
}
void display()
{

cout<<"SIZES OF HEAP"<<setw(30)<<"MOVES" <<endl;
cout<<" "<<endl;
cout<<"A"<<setw(5)<<"B"<<setw(5)<<"C";
cout<<endl;
cout<<a[0]<<setw(5)<<a[1]<<setw(5)<<a[2];
moving();
}
void moving()
{
int elements;
char ch;
char c = getch();
switch(c)
{
case 'A':
ch = 'A';
if(a[0] == 0)
{
moving();
}
else
{
elements = getch();
elements = elements - 48;
a[0] = a[0] - elements;
}
break;
case 'B':
ch = 'B';
if(a[1] == 0)
{
moving();
}
else
{
elements = getch();
elements = elements - 48;
a[1] = a[1] - elements;
}
break;
case 'C':
ch = 'C';
if(a[2] == 0)
{
moving();
}
else
{
elements = getch();
elements = elements - 48;
a[2] = a[2] - elements;
}
break;
case 'E':
exit(0);
break;
default:
moving();
}
turn++;
if(turn % 2 == 0)
{
cout<<setw(21)<<p2<<" HAS MOVED "<<elements<<" FROM " << ch <<endl;
}
else
{
cout<<setw(21)<<p1<<" HAS MOVED "<<elements<<" FROM "<<  ch<<endl;
}
cout<<a[0]<<setw(5)<<a[1]<<setw(5)<<a[2];
if((a[0] ==  0) && (a[1] == 0) && (a[2] == 0) )
{
sleep(1);
ending();
}
else
{
moving();
}
}
void ending()
{
clrscr();
if( turn % 2 ==0)
{
gotoxy(24,10);
cout<<p2<< " HAS WON THE GAME "<<endl;
}
else
{
gotoxy(24,10);
cout<<p1<<" HAS WON THE GAME "<<endl;
}
gotoxy(24,11);
cout<<"THANKS FOR PLAYING NIM GAME "<<endl;
gotoxy(24,12);
cout<<"REGARDS : SAURABH BHATIA CSE (2010 - 2014) "<< endl;
}





