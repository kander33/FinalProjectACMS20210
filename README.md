//FinalProjectACMS20210
#include <iostream>
using namespace std;

//Declaring bool function Contains
bool Contains(string<char> answer,char letter);

int main{

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
  {guess[ii]=" ";
  } else {
  guess[ii]=*;
  }
}

//end of flowchart 1
//start of loop 1

while(wrong<maxwrongguesses){
//Insert DrawHangman function here to output figure to screen
cout << "The number of remaining guesses is " << maxwrongguesses-wrong << end;
//outputting the blank word of *s
cout << guess << endl;
//Ask Player 2 to input the letter to guess
cout << "Player 2: Guess a letter" << endl;
cin >> letter;
//Loop to see if letter is in the answer word



  }
  
  





return 0;
}

//defining bool function Contains
bool Contains(string<char> answer,char letter){
for(int ii=0;ii<answer.size();ii++)
  {
  if(answer[ii]=letter)
    return true;
  }
  return false;
}


