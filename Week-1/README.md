/This folder contains practice codes and Assignment 1 for Week 1.

#include <iostream>
using namespace std;

// function to calculate average
double average( int scores[], int size){
	int sum = 0;
	for (int i= 0; i < size; i++){
		sum += scores[i];
	}
	return (double)sum/size; //return average
}

int main() {
	int userInput;
	cout << "Enter the size of an array: " << endl;
	cin >> userInput;
	
	int scores[userInput] = {90, 85, 70, 95, 100}; // array of 5 elements
	
	cout << "Average = " << average(scores, 5) << endl;
	
	return 0;
	
}
