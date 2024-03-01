## How to build the dashboard step by step ?

#### After importing the csv file into PowerBI, and hitting the ‘transform data’ option which will take you to the Power Query Editor (where we clean the data), here are some tidying up I carried out;

 1. I transformed the "Survived" column by changing 1/0 to Yes/No (makes it more understandable)
 2. I did the same thing to "Pclass" column in replaced 1/2/3 by "First", "Second" and "Third" classes. 
 3. I noticed there were some ‘nulls’ in the age column, for me i didn't deal with them because i did not use the "Age" column in my dashboard. But if you want to use it, here some tips to do:
     - You can replace them all with 0
     - You can fill them using the **median**; because the histograms showed that we have Right-skewed distribution for the column "Age" so using **the mean** to fill missing values is not a good choice in this case, *so the best way to do it is to use the median;*

 4. Replaced S/C/Q in the embarked column with their corresponding names Southampton/Cherbourg/Queenstown. For clarity.
 5. I crosschecked the datatypes for each column and corrected wrongly labelled ones.
 6. Hit Close and Apply

#### Now we are done with the Power Query Editor and we’ve moved to the PowerBI interface where we will write some measures, create new columns and create visuals.

 1. I Created 2 different measures ‘Died’ and ‘Survived’ using the CALCULATE formula. This is so I can distinctively display the number of people who died and survived on the ship.

 2. Created a measure to count the number of passengers present on the ship by using the COUNT formula.

#### Visualization:

 1. Inserted a text box and placed in my title at the top of the page.
 2. I Created 3 different cards to display: a) Total Passengers b) Those who survived c) Those who died.
 3. I Used bar charts to display the number of passengers who survived by a) Gender b) Point of embarkation c) Travel class
 4. I add a pie chart to disply the number of passengers by gender
 5. A doughnut chart for the number of Survived and the number of died

#### After  that, I just did some basic formatting like: 

   - Eliminating the ‘x-axis’ and some ‘y-axis’ and their titles and turning on data labels for each charts.
   - Repositioning the legends.
   - Editing of colors i.e. red to show death and light blue to show survival.
   - Adding titles to each and every chart (it’s very important)
     etc.
