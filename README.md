# coin-calculator
#include <iostream>
#include <iomanip>
using namespace std;
int main() {

	
// Welcome message
    cout << "Welcome to the Coin Cacluator" << endl;
    char redo = false; 
	

//Input for the user
    int pennies;
    int nickles;
    int dimes;
    int quarters;
    int half_dollars;
    int one_dollars;

   
    cout << "Please enter the number of pennies in an amount greater than or equal to zero: " << endl;
    cin >> pennies;
    cout << "Please enter the number of nickles in an amount greater than or equal to zero: " << endl;
    cin >> nickles;
    cout << "Please enter the number of dimes in an amount greater than or equal to zero: " << endl;
    cin >> dimes;
    cout << "PLease enter the number of quarters in an amount greater than or equal to zero: " << endl;
    cin >> quarters;
    cout << "Please enter the amount of half-dollar coins, in an amount greater than or equal to zero: " << endl;
    cin >> half_dollars;
    cout << "Please enter the amount of one-dollar coins, in an amount greater than or equal to zero: " << endl;
    cin >> one_dollars;


//Restating what the user input to make sure that the quantity was right
    cout << "You have " << pennies << " pennies" << endl;
    cout << "You have " << nickles << " nickles" << endl;
    cout << "You have " << dimes << " dimes" << endl;
    cout << "You have " << quarters << " quarters" << endl;
    cout << "You have " << half_dollars << " half-dollar coins" << endl;
    cout << "You have " << one_dollars << " one-dollar coins" << endl;


//calculations
    float total;
    total = pennies * .01 + nickles * .05 + dimes * .10 + quarters * .25 + half_dollars * .50 + one_dollars * 1.0;
    cout << "The value of all of your coins is: $" << total << "." << endl;
