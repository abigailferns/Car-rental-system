#include<iostream>
#include<conio.h>
using namespace std;
class phyprop {
protected:
	char col[50]= [BLUE, BLACK, RED, WHITE, YELLOW, GREEN];
       char bran[50]=[HONDA, JUPITER, SUZUKI, MAESTRO, VESPA, FASCINO];
       char mod[50]=[25S, 6G, CB200X, SP125, PCX160, AX25];
public:
	void getdata() {
		cout << " \n Available choices: \n BLUE, BLACK, RED, WHITE, YELLOW, GREEN. \n Enter Colour: \n";
		cin >> col;
		cout << "Enter Brand: \n";
		cin >> bran;
		cout << "Enter Model: \n";
		cin >> mod;
	}
	
};
class engprop :public phyprop {
protected: int fcap[5]=[13.5L,14L,14.5L,15L,15.5L,16L];
           int ecap[5]=[75cc,120cc,140cc,160cc,200cc, 250cc];
           int hp[5]=[7.6bhp,8.2bhp,9.6bhp,10.2bhp,10.5bhp,11.2bhp];
public:
	void getdata() {
		cout << "Enter required fuel capacity: \n";
		cin >> fcap;
		cout << "Enter required engine capacity: \n";
		cin >> ecap;
		cout << "Enter required horse power: \n";
		cin >> hp;
	}
};
class price : public engprop
{
private: float c=1;
public:
	void cal();
};
void price :: cal()
{
	For(int i=0;i<5;i++)
       {
         If(bran[i] == HONDA)
         { 
           c = c * 200;}
         Elseif(bran[i] == JUPITER){
            C = c * 300}
         Elseif(bran[i] == SUZUKI){
            C = c * 400}

         Elseif(bran[i] == MAESTRO){
            C = c * 500}
         Elseif(bran[i] == VESPA){
            C = c * 600}

        Else{
            C = c * 700}
       }
       

       For(int i=0;i<5;i++)
       {
         If(ecap[i] == 75cc)
         { 
           c = c * 200;}
         Elseif(ecap[i] == 120cc){
            C = c * 300}
         Elseif(ecap[i] == 140cc){
            C = c * 400}

         Elseif(ecap[i] == 160cc){
            C = c * 500}
         Elseif(ecap[i] == 200cc){
            C = c * 600}

         Else{
            C = c * 700}
       }

       For(int i=0;i<5;i++)
       {
         If(hp[i] == 7.6bhp)
         { 
           c = c * 200;}
         Elseif(hp[i] == 8.2bhp){
            C = c * 300}
         Elseif(hp[i] == 9.6bhp){
            C = c * 400}

         Elseif(hp[i] == 10.2bhp){
            C = c * 500}
         Elseif(hp[i] == 10.5bhp){
            C = c * 600}

         Else{
            C = c * 700}
       }

}
Class reg{
Protected: char name[50],add[50];
           Int age[50],phn[50],nod[50];
public:
	void getdata() {
		cout << " Enter Name: \n";
		cin >> name;
		cout << "Enter Address: \n";
		cin >> add;
		cout << "Enter Age: \n";
		cin >> age;
              cout << "Enter Phone no: \n";
		cin >> phn;
              cout << "Enter Number of days: \n";
		cin >> nod;
	}
	
};
