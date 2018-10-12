# turbo-umbrella
#include<stdio.h>
#include<stdlib.h>
#include<conio.h>

int main(void)
{
    
    int vote;
    FILE *fptr;
    
    fptr=fopen("votos.txt","w");
    
    int i,a,b,c,d,e,f;
    a=b=c=d=e=f=0;
    for(i = 1; i <= 5; i++)
    {
        printf("Escolha seu cadito\n");
        printf("1-Candidato A; 2-Candidato B; 3-Candidato C; 4-Candidato; 5-Candidato D\n");
        scanf("%d",&vote);
        fprintf(fptr,"%d\n", vote);
        
        if(vote == 1){
            a++;
        }
        if(vote == 2 ){
            b++;
        }
        if(vote == 3){
            c++;
        }
        if(vote == 4){
            d++;
        }
        if(vote == 5){
            e++;
        }
        
        
    /*fprintf(fptr,"%d\n",a);
    fprintf(fptr,"%d\n",b);
    fprintf(fptr,"%d\n",c);
    fprintf(fptr,"%d\n",d);
    fprintf(fptr,"%d\n",e);
    fprintf(fptr,"%d\n",f);
     */
    }
    fprintf(fptr, "Votos_do_candidato_a: %d\n", a); //Ponteiro do arquivo, mensagem, informações da variavel
    fprintf(fptr, "Votos_do_candidato_b: %d\n", b);
    fprintf(fptr, "Votos_do_candidato_c: %d\n", c);
    fprintf(fptr, "Votos_do_candidato_e: %d\n", d);
    fprintf(fptr, "Votos_do_candidato_f: %d\n", e);
    
    //fclose(vote);
    return 0;
}
