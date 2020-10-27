//# Never-loose-game
//A Simple Computer program in C 

#include <stdio.h>

#include<conio.h>

#include<stdlib.h>

#include<time.h>

int main()

{

  int number,gusses,ngusses=1;
  
  // int gus;
  
  srand(time(0));
  
  number = rand()%100+1;
  
 // printf("the number is %d\n",number);

  do
  
  {  
  
      printf("if you guess this , You will become a CA\n");
      
      printf("guess the number between 1to 100\n");
      
      scanf("%d",&gusses);
      
      if(gusses>number)
      
      {
      
          printf("lower numbder please\n");
      }
      
      
     else if(gusses<number)
      {
      
          printf("higher number plzz\n");
      }
      else
      
      {
          printf("you guess it in %d attempts\n",ngusses);
          
          printf("congraulations you are winner\n");
          
          printf("press any key to exit\n");
      }
      
     // gus=(5-ngusses );
     
     // printf("no of gusses left %d\n",gus);
     
      ngusses++;
  
   }while (gusses!=number);
   
  getch();
  
    return 0;
    
}
