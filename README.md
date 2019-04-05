#include <iostream>
#include <locale.h>
#include "funcao.h"
#include "busca.h"
#include <stdlib.h>
#include <stdio.h>

main()
{
	int r, i, v[10], op, n;
	n=10;
	setlocale(LC_ALL,"portuguese");
	
	for (i=0; i<10; i++)
	{
		printf("Escreva o um numero na posição %d :", i+1);
		scanf("%d", &v[i]);
	}
	system("cls");
	printf("=================== MENU ============================\n");
	printf("=====            1-Pesquisa Sequencial          =====\n");
	printf("=====            2-Pesquisa Binaria             =====\n");
	printf("=====================================================\n");
		scanf("%d",&op);
	
	system("cls");
	
	if(op==1)
	{
		sequencial(v);
	}
	else 
	if(op==2)
	{
		bs(v, n);
			for (i=0; i<10; i++)
		{
			printf("%d/", v[i]);
		}
		printf("\n");
		binaria(v);	
	}
	
}
