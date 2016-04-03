//FinalProjectACMS20210
#include <iostream>
using namespace std;


int main
{

//Defining variables
string answer;
string guess;
int wrong=0;
int maxwrongguesses=6;
char letter;

//input word to guess (answer)
cout << "Player 1: Input word for Player 2 to guess" << endl;
cin >> answer;

//set length of string guess equal to length of answer string
guess.size()=answer.size();

//set word for player 2 to guess (guess string)
for(int ii;ii<guess.size();ii++)
{
if(answer[ii]=" ")
  {
  guess[ii]=" ";
  } 
  else 
  {
  guess[ii]=*;
  }
}

//end of flowchart 1
//start of loop 1






return 0;
}


