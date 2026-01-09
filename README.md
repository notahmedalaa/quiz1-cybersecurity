# quiz1-cybersecurity
a simple code that calculates the bill based on consumption amount / c++
// name / ahmed alaa
//group / A1

#include <iostream>
using namespace std;

int main() {
    int units;
    int unitPrice;
    int bill;
    cout << "please enter the consumption in kilowatt units = ";
    cin >> units;

    if (units <= 100)
        unitPrice = 250;
    else if (units <= 300)
        unitPrice = 300;
    else
        unitPrice = 350;

    bill = units * unitPrice;

    if (bill > 100000)
        cout << "High – reduce usage" << endl;
    else
        cout << "Normal" << endl;

    cout << "Consumption: " << units << endl;
    cout << "Unit Price: " << unitPrice << endl;
    cout << "Total Bill: " << bill << endl;

    return 0;
}
