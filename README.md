#include <stdio.h>
#include <stdlib.h>
void main() {
    char nom[20];
    char prenom[20];
    char mail[80];
    int numero;
        printf ("Entrer le nom \n");
        gets(nom);
            printf ("Entrer le prenom \n");
            gets(prenom);
                printf ("Entrer votre adresse mail \n");
                gets(mail);
                    printf ("Entrer votre numero \n");
                        scanf("%d", &numero);
    
    FILE*f = NULL;
    
    f = fopen("hassantest.txt", "a");
    fprintf (f,"%s;%s;%s;%d", nom, prenom, mail, numero);
    fclose(f);
    printf ("données enregistrer avec succès \n");

    }