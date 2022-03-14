#include <iostream>
using namespace std;
int main()
{
	setlocale(LC_ALL, "Russian");
	cout << "Формирование одномерного массива из матрицы\n\nВведите размер матрицы:\nN=";
	int n = 0;
	cin >> n;
	int** a = new int* [n];
	for (int i = 0; i < n; i++)
	{
		a[i] = new int[n];
	}
	for (int i = 0; i < n; i++)
	{
		for (int j = 0; j < n; j++)
		{
			cout << "a[" << i+1 << "][" << j+1 << "]" << "=";
			cin >> a[i][j];
		}
	}
	cout << "\nИсходная матрица:\n";
	for (int i = 0; i < n; i++)
	{
		for (int j = 0; j < n; j++)
		{
			cout << a[i][j] << " ";
		}
		cout << endl;
	}
	int* massiv = new int[n*n];
	int k = 1;
	cout << "\nПолученный одномерный массив:\n";
	for (int j = ; j ; j)
	{
		for (int i = ; i ; i)
		{
			massiv[k] = a[i][j];
			cout << massiv[k];
			k++;
		}
	}
	cout << endl;

}
