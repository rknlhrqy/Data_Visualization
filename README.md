This document explains that design of this data visualization. It is to show the survival rate of female and male passengers based on different factors, such as passengers' class, age, number of siblings/spouse and number of parents/children.


Summary:

It is well known that gender of the passenger onboard Titanic is related to the survival of passengers. There are also other factors which affect the passenger survival.

In this project, I create the bar chart to show the survival rate of different factors such as Passenger's class (Pclass), Age, Number of Siblings/spouses aboard (SibSp), Number of parents/children aboard (parch), Port of embarkation (Embarked).

Design:

When the customer opens the webpage, a bar chart shows the survival rates of female passengers and male passengers.

Several lines of buttons appears below the bar chart. One line of buttons is for passengers' class (a.k.a Pclass). Each button in this line marks one class. When the customer clicks any button in this line, the bar chart will transition to show the new surival rates of this specific class of female and male passengers.

There are buttons for Siblings/Spouses (a.k.a SibSp), Embarkation port (a.k.a Embarked), and Ages of passengers.

The chart is bar chart. It has two bars. One for female passenger. The other is for male passenger.

The layout is that the bar chart is located at the top. And the buttons are located at the bottom. When you click a button or move the cursor over or away from a button, the color of the button is changed.

The D3.js script will at first do some change on the data. For example, it will put the age into several categories. And these categories will generate all of the age buttons.

It then uses d3.nest() to group the data for different keys. Here Age, Pclass, SibSp, and Embarked are the keys. These data will be later used to generate the bar chart when the customer clicks different buttons.

Then it calls dimple.js function to create the bar chart of the survival rate of female and male passengers in general. This is the bar chart you will see when you first open the webpage.

After that, the script creates the buttons under the bar chart.

And the code will handle the action on the buttons, including clicking th ebutton, moving the curser over the button and moving the cursor away from the button.

Conclusion:

The bar chart shows that:

1, Female passengers in first class has the highest survival rate, 96.81%.

2, The more siblings or spouses the passenger has, less likely he/she survives.

3, Passengers embarking at Port Q have highest survival rate.

4, Female passengers who are older than 60 years all survive.



Feedback:

Not available. Posted on Udacity Forum. And waiting for the feedback. Up to now, no response.

Resources:

1, D3.js API documentation: https://github.com/d3/d3/blob/master/API.md#delimiter-separated-values-d3-dsv

2, Dimple.js documentation: http://dimplejs.org/

3, I also looked through a lot of Dimple.js and D3.js examples about button creating and handling, which I am not able to list here. You can simply goodle them in the internet.

Description of the files:
1, older version of the files are: old_version_index_1.html, old_version_index_2.html, old_version_index_3.html, old_version_index_4.html
2, snapshot of the first version: first_version_09252016.jpg
3, snapshot of the final version: final_version_10052016.jpg
