#include <iostream>
#include <string>
#include <cstdlib>
using namespace std;


char MonName;
void MonAge();
void MonSave();
void MonLoad();
void MonCycle();
void MonWeight();
bool MonSleep = false;
bool MonSick = false; 
void MonHappy();
void MonHunger();
void MonGame();
void MonTalk()
void MonsSleep();
void MonFeed();
void MonPlay();



int main()
{
	//counter
	srand((unsigned)time(0));
	int random_int;
	int lowest=0, highest =5;
	int range=(highest-lowest)+1;
	for(int index=0; index<20; index++)
	{
		random_int = (rand() % range) + lowest/RAND_MAX + 1.0);
		cout << random_int << endl;
	}
	//counter

	//main menu
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
			cout << "The game has been Saved " << endl;
			break;
		case '2':
			MonLoad();
			cout << "You Monster has been Loaded " << endl;
			break;
		case '3':
			MonCycle();
			cout << "Welcome to Matt-a-gotchi" << endl;
			//Option to play game, run through cycle 
			{
				cout << "Please Enter a Name for your Pet" << endl;
				cin >> MonName();
				cout << "The Age of your pet is " << endl;
				cin >> MonAge();
				cout << "The Happiness of your pet is " << endl;
				cin >> MonHappy();

			}
			while count = 0, count < 10, count + 1;
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
					//talking to monster increases happiness by 1 to 3
					// two turns have to pass before you can talk again
					break;
				case '2':
					MonPlay();
					cout << " You are now playing with your Monster " <<  endl;
					cout << "Happiness has been Increased " << endl;
					//Playing with monster increases happiness by 2 to 4, increases hunger by 1 and decreases weight by 1
					//Three turns have to pass before you can play with monster again
					break;
				case '3':
					MonFeed();
					cout << " You are now feeding your Monster " << endl;
					cout << " Your Pets hunger and happiness have increased " << endl;
					//Feeding Monster decreases number of hunger by 3-5, increases weight by 2
					//Four turns have to pass before you can feed again.
					break;
				case '4':
					MonSleep();
					cout << " You have put your Monster to sleep " << endl;
					cout << " Your Monster is now fast asleep " << endl;
					//Monster gets tired after 7 cycles and has to be put to bed within 2 cycles, if not it loses 1-3 both in happiness
					//Monster sleeps for 3 cycles which happiness and weight decrease by 1 and hunger increases by 2
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
			}
			if count = 10
			{
				count = 0;
				MonAge = MonAge + 1;
			}
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

	

	




