//3вариант.Введите массив символов их 23 элементов.Определить, является ли он палиндромом(симметричным с точностью до пробелов)или нет.Например , А РОЗА УПАЛА НА ЛАПУ АЗОРА - палиндром.(Предполагается, что все буквы строки - прописные.)
#include <iostream>
#include <string>
#include <stdlib.h>
#include <time.h>
#include <cmath>
using namespace std;





int main(){
  const int X = 21;
  char Array[X];
  bool Polindrom;
  cout << "Input:";
  for (int i = 0; i <X; i++) {
    //cout << "Input:";
    cin >> Array[i];
  }
  /*for (int i = 0; i < X; i++) {
    cout <<  Array[i];
    
  }*/
  for (int i = 0; i < X; i++) {
    
    if (Array[i] == Array[X-i-1]) {
      Polindrom = true;
      continue;
    }
    else {
      cout << "Not polindrom";
      Polindrom = false;
      break;

    }
    
  }
  if (Polindrom) {
    cout << "Polindrom ";
  }
  

}
