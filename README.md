# NutrifyUMD
An app that scrapes the nutrition facts for every food item from the UMD dining hall menu for a given week and outputs a meal plan to hit the user's dietary goals.

Extra feature:  
Customized meal plans - User inputs their height, weight, BMI, etc. and Nutrify UMD creates a meal plan based on that information + the user's fitness/health goal. You can then ask questions about the meal plan and an AI will answer.

## Example
User inputs:   
body_data: height (6ft), weight(260lb), etc.   
selected_fitness/health_goal: weight loss   
wants_workout_plan?: yes  
  commitment level: 5 days/week, 1 hour/day  

NutrifyUMD output:  
Customized meal plan + detailed workout plan with sets and rest(NutrifyUMD has access to the UMD Gym's equipment list) that fits the users requests  

Reasoning provided by AI model, you can converse with the AI if you want to ask questions about your fitness/health plan.  

## How it works
NutrifyUMD uses the users inputs to calculate the necessary macronutrient (Xg protein, Yg fat, Zg carbs, etc.) & micronutrients (Xmg iron, Ymcg vitamin A, Zmg iodine, etc.) count for a single week.  

Uses linear algebra calculations to get the optimal combination of items in the UMD dining menu to hit the nutrition requirements.  

AI model creates workout routine based on users inputs.

AI model creates reasoning behind the workout + meal plan.

