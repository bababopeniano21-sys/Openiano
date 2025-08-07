#include <iostream>
#include <string>

using namespace std;


int main() {
string myString;
int myChoice;
cout << "Enter Choice 1" << endl;
cout << "[1] List Files"
<< "[2] Create Directory" <<
"[3] change Directory" <<
"[4] Exit"<< endl;
cout << "Enter Choice:" << endl;
cin >> myChoice;


switch (myChoice) {


case 1:
cout << "[1]List all files" << "[2]List by Extension" << "[3]List by Pattern" << endl;
cout << "Enter Choice:";
cin >> myChoice;
cout << "Files in current Directory " << endl;

if(myChoice <= 3) {
cout << "- lab1.cpp" << endl;
cout << "- notes.txt" << endl;
cout << "- data.css" << endl;
}
else {
cout << "error " << endl;
}
break;
case 2:
cout << "Enter Directory name: "<< endl;
cin >> myString;

if ( myString == myString) {
cout << "Directory '" << myString << "' Created Successfully" << endl;
}
else {
cout << "Directory '" << myString << "'has already exist" << endl;
}
break;
case 3:
cout << "Enter choice" << endl;
cout << "[1] Move to parent Directory" << " [2] Move to root Directory" << " [3] Enter custom path " << endl;
cin >> myChoice;
cout << "Enter Path: " << endl;
cin >> myString;

if (myChoice <= 3) {
cout << "Current Directory Changed to:" << myString << endl;

}
else {
cout << "Error: Directory 'invalid path' not found" << myString << endl;

}
break;
case 4:
cout << "Exit" << endl;
break;

default:
cout << "invalid" << endl;
}

return 0;
}
