#include <iostream>
    using namespace std;
                    void faktoriyelHesapla(int num, unsigned long long *result) 
{
    *result = 1;

                  for (int i = 1; i <= num; ++i) {
        *result *= i;
    }
}

        int main() {
    int sayi;
    cout << "Faktöriyelini hesaplamak istediğiniz sayıyı girin: ";
    cin >> sayi;

    unsigned long long sonuc;
    faktoriyelHesapla(sayi, &sonuc);

    cout << sayi << "'nin faktöriyeli: " << sonuc << endl;

    return 0;
