#include <stdio.h>
#include<stdlib.h>
#include<time.h>
void main()

{   system("cls");
    int number,input1,input2,i,computerscore,uscore,cscore; 
    srand(time(NULL));
   printf("\t\t\t\t LET`S PLAY \n");
   printf("1:- STONE\n");
   printf("2:- PAPER\n");
   printf("3:- SCISOR\n");
  
 for (i=0;i<=4;i++)
 {
   printf("\n your input =");
  scanf("%d",&input1);
  printf ("computer input =");
    
    number= (rand()%3)+1;
      printf("%d\n",number);
     if (input1==1&&number==3|| input1 ==2 && number ==1||input1==3 && number==2) 

     {
        printf("hurrah! you won"); 
            uscore+=1;
     }
     else if (1>input1>3)
     {
         printf("enter number between [1-3]");
         
 }

         else if (input1==number)
         {
             printf("tie");

         }
         
       else
       {
          printf("you loose");
          computerscore+=1;
       }       
       }  
       cscore=computerscore-31;
        printf("\n\t\t\t\t YOUR SCORE = %d",uscore);
        printf("\n\t\t\t\t COMPUTER SCORE = %d",cscore);
        
           if (uscore>cscore)
           {
               printf("\t\tyou won");
           }
           else if(uscore<cscore)
           {
             printf("\t\tyou loose"); 
           }
           else
           {
             printf("\t\ttie");
           }
           
    
}
