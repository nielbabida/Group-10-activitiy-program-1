#include <iostream>
#include <string>
using namespace std;

int main() {
    string name;
    int birthYear, birthMonth, birthDay;
    int currentYear = 2025, currentMonth = 2, currentDay = 26;

    cout << "Enter your name: ";
    getline(cin, name);

    cout << "Enter your birth year: ";
    cin >> birthYear;
    cout << "Enter your birth month (1-12): ";
    cin >> birthMonth;
    cout << "Enter your birth day (1-31): ";
    cin >> birthDay;

    int age = currentYear - birthYear - 
        (birthMonth > currentMonth || (birthMonth == currentMonth && birthDay > currentDay));

    cout << "\nYour Name: " << name << endl;
    cout << "Your Age: " << age << " years old" << endl;

    return 0;
}
