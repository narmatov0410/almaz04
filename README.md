#include <iostream>
#include <cmath>
#include <string.h>
#include <ctype.h>
#include <cstdlib>
#include <time.h>
#include <bits/stdc++.h>
#include <cctype>

using namespace std;

//////////////////////////////stringda so`z necha marta takrorlanishi
int main()
{
    string text, res = "";
    getline(cin, text);

    while(text.length()>0){
        int space = text.find(" ");
        string word = text.substr(0, space);
        int index = 0;
        int count = 0;

        while(index < text.length()){
            count++;
            text.erase(index, word.length()+1);
            index = text.find(word);
        }

    cout<< word << ": "<< count <<endl;
}
}
