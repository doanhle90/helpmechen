helpmechen
==========
#include <iostream>
#include <string>
using namespace std;

char MonName;
void MonAge();
void MonSave();
void MonLoad();
void MonCycle();
void MonWeight();
bool MonSleep();
bool MonSick();
void MonHappy();
void MonHunger();
void CycleIncre();
int count();
void MonGame();
void MonTalk()
void MonsSleep();
void MonFeed();
void MonPlay();



int main()
{
  cout << "Welcome to Matt-a-gotchi";
	

	char choice;
	do
	{
	cout << "Matt-a-gotchi" << endl;
	cout << "1 Save Monster" << endl;
	cout << "2 Load Monster" << endl;
	cout << "3 Cycle Monster" << endl;
	cout << "0 Quit Matt-a-gotchi" << endl;
	cout << "Please Enter a selection: " ;
	cin >> choice;

		switch(choice)
		{
		case '1':
			MonSave();
			break;
		case '2':
			MonLoad();
			break;
		case '3':
			MonCycle();
			cout << "Welcome to Matt-a-gotchi" << endl;
			
			{
				cout << "Please Enter a Name for your Pet" << endl;
				cin >> MonName();
				cout << "The Age of your pet is " << endl;
				cin >> MonAge();
				cout << "The weight of your pet is " << endl;
				cin >> MonWeight();
				cout << "The Hunger of your pet is " << endl;
				cin >> MonHunger();
				cout << "The Happiness of your pet is " << endl;
				cin >> MonHappy();

			}
			do while count != 10;
			{
				cout << "What would you like to do with your pet... " << endl;
				cout << "1 Talk " << endl;
				cout << "2 Play " << endl;
				cout << "3 Feed " << endl;
	 			cout << "4 Sleep " << endl;
 				cout << "5 Save " << endl;
				cout << "6 Quit " << endl;
				cin >> option;

				switch(option)
				{
				case '1':
					MonTalk();
					cout << "You have had a Chat with your Monster " << endl;
					cout << "Happiness has been Increased " << endl;
					break;
				case '2':
					MonPlay();
					cout << " You are now playing with your Monster " <<  endl;
					cout << "Happiness has been Increased " << endl;
					break;
				case '3':
					MonFeed();
					cout << " You are now feeding your Monster " << endl;
					cout << " Your Pets hunger and happiness have increased " << endl;
					break;
				case '4':
					MonSleep();
					cout << " You have put your Monster to sleep " << endl;
					cout << " Your Monster is now fast asleep " << endl;
					break;
				case '5': 
					MonsSave();
					cout << " You have now saved your Monster " << endl;
					break;
				case '0':
					cout << "Good Bye " << endl;
					break;
				default: 
					cout << " Invalid, Please select another action... " << endl;
					


				}
			}
			CycleIncre = CycleIncre + 1;
			break;


		case '0':
			cout << "Good Bye " << endl;
			break;
		default:
			cout << " Invalid, Please select another option... " << endl;

			if CycleIncre = 10;
			{
				MonAge = MonAge + 1;
				CycleIncre = 0;
			}
		}
	}

}

	

	


