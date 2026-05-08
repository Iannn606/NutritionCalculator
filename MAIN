
// Nutrition Calculator Version 1 
// Ian Rodriguez

////GLOBAL DEFINITIONS AND LIBRARIES 

#include <stdio.h>  
#include <stdlib.h>
#define maxstrlen 100


//STRUCTURES


//Stores relevant food information for tracking purposes
typedef struct Food{
    char name[maxstrlen];
    int calories;
    int protein;
}Food;

// Stores food information with serving size 
typedef struct Entry
{
    Food food; 
    float servings; // saved as float for awkward serving sizes 1.3, 2.7, etc...
}Entry;


// PROTOTYPES


int main();
int calculate_cal(Entry LOE[]);
int calculate_protein(Entry LOE[]);
void print_summary(int totalcal, int totalpro);


//FUNCTIONS

int calculate_cal(Entry LOE[]){
    int i = 0;
    int totalCal=0;

    while (i>=0 && LOE[i].food.calories !=0){
        if(LOE[i].food.calories == 0){
            break;
        }
        else{
        totalCal = totalCal + LOE[i].food.calories;
        i++;
        }
    }
    return totalCal;
    
}
    
int calculate_protein(Entry LOE[]){
    int i = 0;
    int totalpro = 0;

    while (i>=0 && LOE[i].food.protein != 0){
        if (LOE[i].food.protein == 0){
            break;
        }
        else{
            totalpro = totalpro + LOE[i].food.protein;
            i++;
        }
    }
    return totalpro;
}

void print_summary(int totalcal, int totalpro){
    printf("Total calories consumed: %d", totalcal);
    printf("\nTotal protein consumed: %d", totalpro);
}

int main(){
    Entry LOE[maxstrlen]={0};//Fixed size list of entries 
    int stop = 0;
    int i = 0;

    //set up food 
    while( i>=0 & stop ==0){
    
        printf("what food would you like to add?");
        scanf("%s",LOE[i].food.name);


        printf("Perfect, now how many calories are in a serving?");
        scanf("%d",&LOE[i].food.calories);

        printf("How much protein is in a serving?");
        scanf("%d", &LOE[i].food.protein);

        i++;

        printf("if you are done type 1 if you wish to continue type 0 ");
        scanf("%d", &stop);
        if(stop){ 
            int totalcal = calculate_cal(LOE);
            int totalpro = calculate_protein(LOE);
            print_summary(totalcal, totalpro);
            break;
        }
    } 
}

