---
layout: post
title: Digimon
subtitle: Lab 1
cover-img: /assets/img/DigimonBackground.jpg
thumbnail-img: /assets/img/DigimonLogo.png
share-img: /assets/img/DigimonLogo.png
tags: [digimon,labs]
---

In order to calculate the average speed of the digimons, I used a for loop to add each digimon’s speed to a “total” variable and also add one to a “count” variable to keep track of the number of digimons. I then calculated the mean by dividing these two variables.

For the second problem, I knew initially that the function would have to have two parameters – one for the category of the attribute and one for the attribute itself. The function creates a main dictionary. Then, in the main dictionary, it creates a key for each specific attribute (ex. Vaccine) within the input category (ex. Type). Each digimon is then counted according to its attribute. Finally, the value associated with the specific input attribute is printed. One thing that could be improved in my function is ensuring the capitalization of the input matches the capitalization of the category without checking manually.

The third problem was a bit trickier for me. My initial plan was to create a dictionary of all of the digimons, pick two randomly, and then iterate through the rest to find a third that met the memory and attack requirements for that team. Below is some code that I started to write:

{% highlight python linenos %}
count = 1
memory = 0
attack = 0
team = {}

for row in data:
   total[count] = row
   count += 1

one = random.randint(1, 250)
two = random.randint(1, 250)
team[1] = main[one]
team[2] = main[two]

for i in range(1,3):
   memory += int(team[i]["Memory"])
   attack += int(team[i]["Atk"])

if memory > 13:
   if team[1]["Memory"] > team[2]["Memory"]:
       memory -= int(team[1]["Memory"])
       del team[1]
   else:
       memory -= int(team[2]["Memory"])
       del team[2]
{% endhighlight %}

I quickly found that this method was going to be too complicated and unnecessary, so instead I decided to use nested for loops. There are three for loops and each for loop finds a unique digimon. The innermost for loop then totals the memory and attack values and checks to see if they match the requirements. After I created code that returned a team of digimons successfully, I noticed that the system would pick the same team each time because that was the first team that it encountered. In order to pick a random team each time, I went back to the start of the function and randomized the order of the digimons by associating the digimon with a random key value. In finding a random team, I learned how to use the random.sample command - [here is my source] (https://stackoverflow.com/questions/22842289/generate-n-unique-random-numbers-within-a-range).
