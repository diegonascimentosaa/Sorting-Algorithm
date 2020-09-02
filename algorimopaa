#include <iostream>
using namespace std;
void mostrar(int vet[], int tam)
{
    int i=0;
    while(i < tam)
    {
        cout << vet[i] << " , ";
    i++;
    }
}

int particao(int vet[], int esq, int dir)
{
    int aux;
    int j = esq;
    int pivo = vet[dir];
    int i = (esq - 1);
    while(j < dir)
    {

        if (vet[j] <= pivo)
        {
            i++;
            aux = vet [j];
            vet [j] = vet [i];
            vet [i] = aux;
        }
        j++;
    }
    i++;
    aux = vet [dir];
    vet [dir] = vet [i];
    vet [i] = aux;
    return i;
}

void quickSort(int vet[], int esq, int dir)
{
    if (esq < dir)
    {
        int pivo = particao(vet, esq, dir);
        quickSort(vet, esq, pivo - 1);
        quickSort(vet, pivo + 1, dir);
    }
}
int main()
{
    int vet[] = { 9, 10, -1, 3, 6, 2, 1, -3, 1, 0, -2, 15, 8, -7, 0 };
    int tam;

    tam  = sizeof(vet) / sizeof(vet[0]);
    cout << "O vet original e: ";
    mostrar(vet, tam);
    cout << endl;
    quickSort(vet, 0, tam);
    cout << "O vet ordenado e: ";
    mostrar(vet, tam);
    cout << endl;
}
