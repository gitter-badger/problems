```cpp
#include <iostream>
#include <string>
using namespace std;

void printMovies(string title, string director, int year, int time);

struct MovieData
{
	string title;
	string director;
	int yearReleased;
	int runningTime; //In Minutes

};

int main()
{	
	MovieData disney, pixar;

	disney.title = "Toy Story";
	disney.director = "Juanito";
	disney.yearReleased = 2012;
	disney.runningTime = 120;

	pixar.title = "Cars";
	pixar.director = "Juanito Gonzales";
	pixar.yearReleased = 2010;
	pixar.runningTime = 124;
	
	printMovies(disney.title, disney.director, disney.yearReleased, disney.runningTime);

	cout << endl;
	printMovies(pixar.title, pixar.director, pixar.yearReleased, pixar.runningTime);

	system("pause");
	return 0;
}

void printMovies(string title, string director, int year, int time)
{
	cout << "Title: " << title << endl
		<< "Director: " << director << endl
		<< "Year Released: " << year << endl
		<< "Running Time: " << time << endl;
}

```
## Computer Science Problems

- [From 1 - 10](1-10)
- [From 11 - 20](11-20)
- [From 21 - 30](21-30)
- [From 31 - 40](31-40)
- [From 41 - 50](41-50)
- [From 51 - 60](51-60)


Kinetic Energy
In physics, an object that is in motion is said to have kinetic energy. The following formula can be used to determine a moving object’s kinetic energy:



The variables in the formula are as follows: KE is the kinetic energy in joules, m is the object’s mass in kilograms, and v is the object’s velocity in meters per second. Write a function named kineticEnergy that accepts an object’s mass (in kilograms) and velocity (in meters per second) as arguments. The function should return the amount of kinetic energy that the object has. Demonstrate the function by calling it in a program that asks the user to enter values for mass and velocity.

Winning Division
Write a program that determines which of a company’s four divisions (Northeast, Southeast, Northwest, and Southwest) had the greatest sales for a quarter. It should include the following two functions, which are called by main.
• double getSales() is passed the name of a division. It asks the user for a division’s quarterly sales figure, validates the input, then returns it. It should be called once for each division.
• void findHighest() is passed the four sales totals. It determines which is the largest and prints the name of the high grossing division, along with its sales figure.
Input Validation: Do not accept dollar amounts less than $0.00.

Safest Driving Area
Write a program that determines which of 5 geographic regions within a major city (north, south, east, west, and central) had the fewest reported traffic accidents last year. It should have the following two functions, which are called by main.
• int getNumAccidents() is passed the name of a region. It asks the user for the number of traffic accidents reported in that region during the last year, validates the input, then returns it. It should be called once for each city region.
• void findLowest() is passed the five accident totals. It determines which is the smallest and prints the name of the region, along with its accident figure.
Input Validation: Do not accept an accident number that is less than 0.
Lowest Score Drop
• Write a program that calculates the average of a group of test scores, where the lowest score in the group is dropped. It should use the following functions:
• void getScore() should ask the user for a test score, store it in a reference parameter variable, and validate it. This function should be called by main once for each of the five scores to be entered.
• void calcAverage() should calculate and display the average of the four highest scores. This function should be called just once by main, and should be passed the five scores.
• int findLowest() should find and return the lowest of the five scores passed to it. It should be called by calcAverage, which uses the function to determine one of the five scores to drop.
Input Validation: Do not accept test scores lower than 0 or higher than 100.

Star Search
A particular talent competition has 5 judges, each of whom awards a score between 0 and 10 to each performer. Fractional scores, such as 8.3, are allowed. A performer’s final score is determined by dropping the highest and lowest score received, then averaging the 3 remaining scores. Write a program that uses these rules to calculate and display a contestant’s score. It should include the following functions:
• void getJudgeData() should ask the user for a judge’s score, store it in a reference parameter variable, and validate it. This function should be called by main once for each of the 5 judges.
• double calcScore() should calculate and return the average of the 3 scores that remain after dropping the highest and lowest scores the performer received. This function should be called just once by main, and should be passed the 5 scores.
The last two functions, described below, should be called by calcScore, which uses the returned information to determine which of the scores to drop.
• int findLowest() should find and return the lowest of the 5 scores passed to it.
• int findHighest() should find and return the highest of the 5 scores passed to it.
Input Validation: Do not accept judge scores lower than 0 or higher than 10.

Order Status
The Middletown Wholesale Copper Wire Company sells spools of copper wiring for $100 each and ships them for $10 apiece. Write a program that displays the status of an order. It should use two functions. The first function asks for the following data and stores the input values in reference parameters.
• The number of spools ordered.
• The number of spools in stock.
• Any special shipping and handling charges (above the regular $10 rate).
The second function receives as arguments any values needed to compute and display the following information:
• The number of ordered spools ready to ship from current stock.
• The number of ordered spools on backorder (if the number ordered is greater than what is in stock).
• Total selling price of the portion ready to ship (the number of spools ready to ship times $100).
• Total shipping and handling charges on the portion ready to ship.
• Total of the order ready to ship.
The shipping and handling parameter in the second function should have the default argument 10.00.
Input Validation: Do not accept numbers less than 1 for spools ordered. Do not accept a number less than 0 for spools in stock or for shipping and handling charges.

Overloaded Hospital
Write a program that computes and displays the charges for a patient’s hospital stay. First, the program should ask if the patient was admitted as an in-patient or an out-patient. If the patient was an in-patient the following data should be entered:
• The number of days spent in the hospital
• The daily rate
• Charges for hospital services (lab tests, etc.)
• Hospital medication charges.
If the patient was an out-patient the following data should be entered:
• Charges for hospital services (lab tests, etc.)
• Hospital medication charges.
The program should use two overloaded functions to calculate the total charges. One of the functions should accept arguments for the in-patient data, while the other function accepts arguments for out-patient data. Both functions should return the total charges.
Input Validation: Do not accept negative numbers for any information.

Population
In a population, the birth rate is the percentage increase of the population due to births and the death rate is the percentage decrease of the population due to deaths. Write a program that asks for the following:
• The starting size of a population
• The annual birth rate
• The annual death rate
• The number of years to display
The program should then display the starting population and the projected population at the end of each year. It should use a function that calculates and returns the projected new size of the population after a year. The formula is

N = P(1 + B)(1 - D)

where N is the new population size, P is the previous population size, B is the birth rate, and D is the death rate.

Input Validation: Do not accept numbers less than 2 for the starting size. Do not accept negative numbers for birth rate or death rate. Do not accept numbers less than 1 for the number of years.
