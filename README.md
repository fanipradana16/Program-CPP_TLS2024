# Program-CPP_TLS2024
The program is used to calculate a discount.
#include <iostream>
#include <iomanip>  // Untuk std::setprecision
using namespace std;

int main() 
{
    // Deklarasi variabel
    double hargaAsli, persentaseDiskon, hargaDiskon, jumlahDiskon;

    // Input dari pengguna
    cout << "Masukkan harga asli: Rp ";
    cin >> hargaAsli;

    cout << "Masukkan persentase diskon (dalam %): ";
    cin >> persentaseDiskon;

    // Menghitung diskon
    jumlahDiskon = hargaAsli * (persentaseDiskon / 100.0);
    hargaDiskon = hargaAsli - jumlahDiskon;

    // Menampilkan hasil
    cout << std::fixed << std::setprecision(2); // Format angka dengan dua desimal
    cout << "Jumlah diskon: Rp " << jumlahDiskon << std::endl;
    cout << "Harga setelah diskon: Rp " << hargaDiskon << std::endl;

    return 0;
}
