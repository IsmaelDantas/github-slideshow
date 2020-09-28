#include <iostream>
#include <cstdlib>
using namespace std;
int main(){
	int n1=0;
	int n2=0;
	int res=0;
	char nome[50];
	char opc;
	
	inicio:
	system("cls");
				
				
	cout << "Digite o Nome do Aluno  " << "\n" << "\n";
	cin >> nome;
	cout << "Nome do Aluno: "<< nome << "\n";
	cout << "Digite a primeira nota do Aluno(a) " << nome << "\n" << "\n";
	cin >> n1;
	cout << "Digite a segunda nota do Aluno(a) " << nome << "\n" << "\n";
	cin >> n2;
	res=(n1+n2)/2;
	cout << "Resultado Final:  " << res << "\n\n";
	if(res>=7){
		cout << "Aluno(a) Aprovado(a)" << "\n\n";
	}else if (res>=3)
	{
		cout << "Aluno(a) em Recuperação" << "\n\n";
	}else
	{
		cout << "Aluno(a) Reprovado(a)" << "\n\n";
	}
	
	cout << "\nDigitar outras notas?\n[s/n]:  ";
	
	cin >> opc;
	
	if(opc == 's' or opc == 'S')
	{
	
		goto inicio;
	}
	
			
	return 0;
}


