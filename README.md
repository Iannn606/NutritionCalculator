# Nutrition Calculator (Version 1) 

## Goal
The goal is to create a simple C program that will use input to create a summary of my selected nutrition (protein and Calories) for the day

## Features
- Add calories total
- Add Protein total
- Ask for food nutrition through the command line
- Display Nutrition Info in a polished summary 

## Constraints
some examples of what i will NOT be including in this current version is
- any API
- dynamic memory techniques/algorithms or space saving pointers for efficiency 
- recommendation systems
- UI/Web interface implementation (Version 1 will stay on the command line)
- any modification handling 
- I will be hardcoding data (100 generic foods) from reputable 3rd parties (USDA FoodData Central). it will be generic food (not brand specific) information for now. it also will not be complete descriptions like listed on the actual website. 


## Additional Technical information 
- Each serving will be "one unit" which i will be defining as equal to 100g for ALL food, I wont be accounting for varying serving sizes just yet (the expectation is to calculate how many servings you ate yourself).
- If looking at the data on the third part site i will be using "energy: atwater general" for calorie information
- Calories and protein will be rounded to the nearest integer (EX: 0.5 -> 1 , 2.4 -> 2)
