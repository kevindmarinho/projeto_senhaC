# projeto_senhaC
Projeto de senhas pre-determinadas em linguagem C.

#include <stdio.h>
#include <stdlib.h>
#include<locale.h>
#include<string.h>

 

 int main()    
{
	int choice,cargo;
    char senha[5];
    char Diretor[4]={'d', '0', '1', '0'},SupervisorGeral[4]={'b','0','2','9'},Supervisor[4]={'b','0','2','0'},Gerente[4]={'b','8','2','0'},funcionario[4]={'b','0','1','1'};
    
	setlocale(LC_ALL,"Portuguese_Brazil");
	
	 
 printf("**BEM VINDO AO PROGRAMA*\n"); system("color 9"); 
 printf("\n Escolha uma opção: \n(1)Entrar \n(2)Criar uma senha\n");
 scanf("%d",&choice);
 system("cls");
   if (choice==1){
   
 printf("\nPor favor, Digite sua senha:");
    scanf("%s",&senha);
    system("cls");

    if (strcmp(senha,Diretor) == 0)
    {
         printf("\n\n\n\n    * Ola, Diretor! Seja Bem Vindo! *\n\n\n"); system("color 9F");
         printf("  ---------->> Voce tem acesso aos setores A,B e C <<----------\n\n\n\n\n\n");
                 }
                 
    else if (strcmp(senha,SupervisorGeral) == 0)
    {
         printf("\n\n\n\n    * Ola, Supervisor Geral **\n\n");system("color 9F");
         printf("  ----------->> Voce tem acesso aos setores A e B <<----------\n\n\n\n");
         }
         
    else if (strcmp(senha,Supervisor) == 0)
    {
         printf("\n\n\n\n    * Ola, Supervisor! *\n\n\n\n");system("color 9F");
         printf("  ---------->> Voce tem acesso ao setor B <<----------\n\n\n\n\n");
        }            
   
    else if (strcmp(senha,Gerente) == 0)
    {
         printf("\n\n\n\n    * Ola, Gerente! *\n\n\n\n");system("color 9F");
         printf("  ---------->> Voce tem acesso aos setores A e C  <<----------\n\n\n\n");
        }
    else if (strcmp(senha,funcionario) == 0)
    {
        printf("\n\n\n\n     * Ola, Funcionario! *\n\n\n\n");system("color 9F");
        printf("   ---------->> Voce tem acesso ao setor C <<----------\n\n\n\n");
}
    else
    {system("color cF");
    printf("\n\n\n\n              !!!!!!!!!!!Senha incorreta. Acesso Negado!!!!!!!!!!!!!!\n\n\n\n");}
 
}  else{
    
  printf("Por favor, digite a opção equivalente ao seu cargo. \n(1) Diretor. \n(2)Supervisor Geral. \n(3)Supervisor. \n(4)Gerente. \n(5)funcionario.\n");
  scanf("%d",&cargo);
  system("cls");
  
        if (cargo==1){
         system("color C");	
       	printf("Sua nova senha será:\n d010\n ");
	   }
	   else if (cargo==2){
	   	system("color C");
	   	printf("Sua nova senha será:\n b029\n");
	   }
       else if (cargo==3){
       	system("color C");
	   	printf("Sua nova senha será:\n b020\n");
	   }
       else if (cargo==4){
       	system("color C");
	   	printf("Sua nova senha será:\n b820\n");
	   }
	   else if (cargo==5){
	   	system("color C");
	   	printf("Sua nova senha será:\n b011\n");  
        }
       else
           {system("color cF");
           printf("\n\n\n\n              !!!!!!!!!!!NENHUMA OPÇÃO SELECIONADA. TENTE NOVAMENTE!!!!!!!!!!!!!!\n\n\n\n");}
  
   

}


    system("pause");
    return 0;
}

