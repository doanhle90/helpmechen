#include <iostream>
#include <string>
#include <cstdlib>
#include <ctime>
using namespace std;

void MonSave();
void MonLoad();
void MonCycle();
void MonWeight();
void MonHappy();
void MonHunger();
void MonGame();
void MonTalk()
void MonSleep;
void MonFeed();
void MonPlay();
void MonPlayTime();


int main()
{
srand((unsigned)time(0));
int choice;
int MonChoice = (rand()%3)+1;
int PlayerScore;
int MonsterScore;
char MonName;
int MonAge;
bool MonSleep = false;
bool MonSick = false; 
int random_int;
int lowest=0, highest =5;
int range=(highest-lowest)+1;

//counter
	
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
			 	fstream myfile;
				myfile.open ("savedMonster.txt");
				myfile << MonName << endl << MonWeight << endl << MonHunger << endl << MonAge << endl;
				myfile.close();
				cout << "Your Monster Has been Saved" << endl;
				break;
		case '2':
			MonLoad();
				fstream myfile;
				myfile.open ("savedMonster.txt");
				myfile >> MonName;
				myfile >> MonAge;
				myfile >> MonHunger;
				myfile >> MonWeight;
				cout << "\nWelcome back to " << MonName << " Your Monsters Profile " <<"\nAge:" MonAge << "/nHunger" << MonHunger << "/nWeight" << Monweight;
				myfile.close();
				cout << "You Monster has been Loaded " << endl;

			break;
		case '3':
			cout << "Please Enter a Name for your Pet" << endl;
			cin >> MonName();
			MonCycle();
			cout << "Welcome to Matt-a-gotchi" << endl;
			//Option to play game, run through cycle 
			{
				cout << "The Age of your pet is " << endl;
				cin >> MonAge();
				cout << "The Happiness of your pet is " << endl;
				cin >> MonHappy();

			}
		
			while (count = 0, count < 10, count + 1;
			{
				cout << "What would you like to do with your pet... " << endl;
				cout << "1 Talk " << endl;
				cout << "2 Play " << endl;
				cout << "3 Feed " << endl;
	 			cout << "5 Sleep " << endl;
				cout << "6 Save " << endl;
				cout << "7 Quit " << endl;
				cin >> option;

				switch(option)
				{
				case '1':
					MonTalk();
					cout << "You have had a Chat with your Monster " << endl;
					cout << "Happiness has been Increased " << endl;
					{
						random_int = rand() % range) + lowest/RAND_MAX + 1.0);
						cout << random_int << endl;
						MonHappy = MonHappy - random_int;
					}

					cout <<  MonHappy << endl;
					count = count + 1;
					//talking to monster increases happiness by 1 to 3
					// two turns have to pass before you can talk again
					break;
				case '2':
					MonPlay();
					cout << " You are now playing with your Monster " <<  endl;
					cout << "Happiness has been Increased " << endl;
					{
						random_int = rand() % range) + lowest/RAND_MAX + 1.0);
						cout << random_int << endl;
						MonHappy = MonHappy + random_int;
						MonHunger = MonHunger + 1;
						MonWeight = MonWeight - 1;

						cout << MonHappy << endl;
						cout << MonHunger << endl;
						cout << MonWeight << endl;
						
						count = count + 1;

					}
					//Playing with monster increases happiness by 2 to 4, increases hunger by 1 and decreases weight by 1
					//Three turns have to pass before you can play with monster again
					break;
				case '3':
					MonFeed();
					cout << " You are now feeding your Monster " << endl;
					cout << " Your Pets hunger and happiness have increased " << endl;
					{
						random_int = rand() % range) + lowest/RAND_MAX + 1.0);
						MonHunger = MonHunger - random_int;
						MonWeight = MonWeight + 2;
					}
					count = count + 1;
					
					//Feeding Monster decreases number of hunger by 3-5, increases weight by 2
					//Four turns have to pass before you can feed again.
					break;
				case '4':
					MonPlayTime();
					cout << "Its time to play! " << endl;
					cout << "Welcome to Fire, Earth, Wind and Water!";
				    cout << "Lets begin. You are playing against your Monster. ";
				    cout << "Type 0 for Fire, 1 for Earth,2 for Wind, and 3 for Water\n";
				    cin >> choice;
				do{
					if (choice == 0)
					{
						if (MonChoice == 0)
						cout << " Fire Ties with Fire, Its a Draw! " << endl;
						else if (MonChoice == 1)
						cout << " Fire beats Earth! You WIN! " endl;
						PlayerScore = PlayerScore + 1;
						else if (MonChoice == 2)
						cout << " Fire draws with Wind! It's a Draw! " endl;
						else if (MonChoice == 3)
						cout << " Fire Loses to Water! You LOSE! " endl;;
						MonsterScore = MonsterScore + 1;
					}
					if (choice == 1)
					{
						if (MonChoice == 0)
						cout << " Earth Loses to Fire! You LOSE! " << endl;
						MonsterScore = MonsterScore + 1;
						else if (MonChoice == 1)
						cout << " Earth Ties with Earth!, It's a Draw! " endl;
						else if (MonChoice == 2)
						cout << " Earth Beats Wind! You WIN! " endl;
						PlayerScore = PlayerScore + 1;
						else if (MonChoice == 3)
						cout << " Earth Ties with Water, It's a Draw " endl;;
					}
					if (choice == 2)
					{
						if (MonChoice == 0)
						cout << " Wind draws with Fire, It's a Draw " endl;
						if (MonChoice == 1)
						cout << " Wind Loses to Earth, You LOSE! " endl;
						MonsterScore = MonsterScore + 1; 
						if (MonChoice == 2)
						cout << " Wind draws with Wind, It's a Draw " endl;
						if (MonsChoice == 3)
						cout << " Wind Beats Water, You WIN! " endl;
						PlayerScore = PlayerScore + 1;
					}
					if (choice == 3)
					{
						if (MonChoice == 0)
						cout << "Water Beats Fire, You WIN! " endl;
						PlayerScore = PlayerScore + 1;
						if (MonChoice == 1)
						cout << " Water draws with Earth, It's a Draw! " endl;
						if (MonChoice == 2)
						cout << " Water Loses to Wind, You Lose! " endl;
						MonterScore = MonsterScore + 1;
						if (MonsChoice == 3)
						cout << " Water draws with Water, It's a Draw! " endl;
					
					}

				}
				while(PlayerScore < 5 && MonsterScore < 5)
				if(PlayerScore == 5)
				{
					cout << "You are the Winner! " << endl;
					MonHappy = MonHappy + 2
				}
				if(MonsterScore == 5)
				{
					cout << "You Lose, Your Monster Wins! " << endl;
					MonHappy = MonHappy + 4
				}
					MonWeight = MonWeight - 1;
					MonHunger = MonHunger + 2;
					//If monster loses happiness increases by 2 if monster wins it increases by 4
					//Weight still decreases by 1 and hunger increases by 2
					//You can only play with your pet every 3rd turn
					break;
				case '5':
					MonSleep();
					cout << " You have put your Monster to sleep " << endl;
					cout << " Your Monster is now fast asleep " << endl;
					
					MonHappy = MonHappy - 1;
					MonWeight = MonWeight - 1;
					MonHunger = MonHunger + 2;
					
					if(count = 8)
					{
						count = 1;
						MonAge = MonAge + 1;
					}
					else if (count = 9)
					{
						count = 2;
						MonAge = MonAge + 1;
					}
					count = count + 3;
					//Monster gets tired after 7 cycles and has to be put to bed within 2 cycles, if not it loses 1-3 both in happiness
					//Monster sleeps for 3 cycles which happiness and weight decrease by 1 and hunger increases by 2
					break;
				case '6': 
					MonSave();
					 	fstream myfile;
						myfile.open ("savedMonster.txt");
						myfile << MonName << endl << MonWeight << endl << MonHunger << endl << MonAge << endl;
						myfile.close();
						cout << "Your Monster Has been Saved" << endl;
						cout << " You have now saved your Monster " << endl;
						break;
				case '7':
					cout << "Good Bye " << endl;
					break;
				default: 
					cout << " Invalid, Please select another action... " << endl;
				}	


				}
			}
			if count = 10 // counter counts to 10 then once it hits ten the monster age goes up by 1 day and count resets to 0
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

			
			
		}
	}

}

	

	




