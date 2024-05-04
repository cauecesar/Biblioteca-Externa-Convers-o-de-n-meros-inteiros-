#include <iostream>
using namespace  std;
#include <boost/dynamic_bitset.hpp>

string intParaBinario(int numero) {
    boost::dynamic_bitset<> bits(8, numero); 
    return bits.to_string(); 
}

int main() {
    int numero;

    cout << "Digite um número inteiro: ";
    cin >> numero;

    string binario = intParaBinario(numero); 

    cout << "O número " << numero << " em binário é: " << binario << endl;

    return 0;
}
