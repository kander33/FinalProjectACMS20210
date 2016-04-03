//FinalProjectACMS20210
#include <iostream>
#include <string>
using namespace std;

//Declaring bool function Contains
bool Contains(string answer,char letter);

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

while(wrong<maxwrongguesses)
{
//Output Hangman figure to the screen
void DrawHangman(int wrong);
 {
 if (wrong==0)
  {
  cout<<""+====== "<<endl;
 	cout<<"|   |   "<<endl;
 	cout<<"|       "<<endl;
 	cout<<"|       "<<endl;
 	cout<<"|       "<<endl;
 	cout<<"========";<<endl;
  }
 elseif (wrong==1)
  {
  cout<<""+====== "<<endl;
 	cout<<"|   |   "<<endl;
 	cout<<"|   O   "<<endl;
 	cout<<"|       "<<endl;
 	cout<<"|       "<<endl;
 	cout<<"========";<<endl;
  	}
 elseif (wrong==2)
  {
  cout<<""+====== "<<endl;
 	cout<<"|   |   "<<endl;
 	cout<<"|   O   "<<endl;
 	cout<<"|   |   "<<endl;
 	cout<<"|       "<<endl;
 	cout<<"========";<<endl;
 	}
 elseif (wrong==3)
  {
  cout<<""+====== "<<endl;
 	cout<<"|   |   "<<endl;
 	cout<<"|   O   "<<endl;
 	cout<<"|  /|   "<<endl;
 	cout<<"|       "<<endl;
 	cout<<"========";<<endl;
 	}
 elseif (wrong==4)
 {
 cout<<""+====== "<<endl;
 	cout<<"|   |   "<<endl;
 	cout<<"|   O   "<<endl;
 	cout<<"|  /|\    "<<endl;
 	cout<<"|       "<<endl;
 	cout<<"========";<<endl;
 	}
 elseif (wrong==5)
 {
  cout<<""+====== "<<endl;
 	cout<<"|   |   "<<endl;
 	cout<<"|   O   "<<endl;
 	cout<<"|  /|\    "<<endl;
 	cout<<"|  /    "<<endl;
 	cout<<"========";<<endl;
 	}
 }
cout << "The number of remaining guesses is " << maxwrongguesses-wrong << end;
//outputting the blank word of *s
cout << guess << endl;
//Ask Player 2 to input the letter to guess
cout << "Player 2: Guess a letter" << endl;
cin >> letter;
//Loop to see if letter is in the answer word
if(Contains(answer,letter)=1)
  {
  cout << "Letter is in word" << endl;
  for(int i=0;i<answer.size();i++)
  {
    if(answer[i]==letter)
      guess[i]=letter;
    }
  } 
  else 
  {
    wrong++;
    cout << "Sorry, letter guessed is not in the word" << endl;
    cout << "Number of guesses left is " << maxwrongguesses-wrong << endl;
  }
if(guess==answer){
  cout << "Congratulations!  You guessed the correct word" << endl;
  break;
  }

}
  

return 0;
}

//defining bool function Contains
bool Contains(string answer,char letter)
{
for(int ii=0;ii<answer.size();ii++)
  {
  if(answer[ii]=letter)
    return true;
  }
  return false;
}


