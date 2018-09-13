#include <iostream>
#include <string.h>

using namespace std;


int diagsum (void);
int x=0;
int y=2;

int main()
{

    diagsum ();
    return 0;
}


int diagsum (void)
{
    int matr[3][3] = {{1,2,3},{4,5,6},{7,8,9}};

    int n = 3;
    int sumad1 = 0;
    int sumad2 = 0;
    int sumat;

    for (int i=0; i<3; i++)
    {
            //cout<<"matrix["<<i<<"]["<<i<<"]: " <<matr[i][i]<<endl;
            sumad1 = sumad1+matr[i][i];
            cout<< "suma de diagonal 1 es: "<< sumad1<< endl;



    }

    for (int j=0; j<3; j++)
    {


            //cout<<"matrix["<<x<<"]["<<y<<"]: " <<matr[x][y]<<endl;
            sumad2 = sumad2+matr[x][y];
            cout<< "suma de diagonal 2 es: "<< sumad2<< endl;
            x++;
            y--;


    }

     sumat= sumad1 + sumad2;

    cout<< "la suma de las diagonales es: "<< sumat<< endl;
}
