#include <iostream>
using namespace std;
//função para mostrar o vetor
void mostrar(int vet[], int tam) {
  int i;
  for (i = 0; i < tam; i++) {
    cout << vet[i] << " , ";
  }
}
//função de ordenação insertion sort
void algoritmoinsertionsort(int vet[], int tam) {
  int a, chave, j;
  for (a = 1; a < tam; a++) {
    chave = vet[a];
    j = a - 1;
    while (chave < vet[j] && j >= 0) {
      vet[j + 1] = vet[j];
      --j;
    }
    vet[j + 1] = chave;
  }
}

int main()
{
    int vet[] = { 9 , 10 , -1, 3, 6, 2, 1, -3, 1, 0, -2, 15, 8, -7, 0 };
    int tam = 15; 
    cout << "O vetor original e: "; //
    mostrar(vet, tam);
    cout << endl;
    algoritmoinsertionsort(vet, tam);
    cout << "O vetor ordenado e: ";
    mostrar(vet, tam);
    cout << endl;
    return 0;
}
