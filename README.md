
#include <iostream>
using namespace std;
int main()
{
    int n;
    cout << "Vvedite skolko znacheniy v massive";
    cin >> n;
    int * mas = new int [n];
    for (int i=0;i<n;i++)
    {
        mas[i] = rand()%100;
    }
    for (int i=0;i<n;i++)
    cout << mas[i] << endl;
    for (int i=0;i<n;i++)
     for(int j=0;j<n-1;j++)
        if(mas[i]>mas[i+1])
        {
            int temp = mas [i+1];
            mas[i+1]=mas[i];
            mas[i]=temp;
            
            
        }
        cout <<  "\n";
        for (int i=0;i<n;i++)
        cout << mas[i] << "\n";
    return 0;
}
