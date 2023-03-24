# YouTube Trending Videos (EDA)

<p align="center">
<img src = 'https://cdn.searchenginejournal.com/wp-content/uploads/2020/12/top-trending-featured-image-5fcf26c0867f6-768x403.png' width='800' height='400'> 
</p>

Company that I've recently applied to provided me with the task I'm going to outline here:

--- 

```
Based on https://kaggle.com/datasnaek/youtube-new answer these questions:

	•	What are the categorical differences in viewing patterns between Germans and Indians?

	•	Ratios between views / likes / dislikes for different categories / countries. 

	•	Сhannels that are popular in most countries.
```
---

I had to showcase my ```Python``` skills, manipulating ```JSON``` files (since they use ```MongoDB```) and data visualization via ```Tableau```. 

Due to the *\"competitive nature of the hiring process\"*, they've obviosly looked for the nuances and honestly I've failed because I didn't understood the data completely.

When I say "completely", I'm not going to be biased and say that those are "noobish" nor "professional" mistakes. Probably, on the job, these could be fixed before going into production. Everyone makes mistakes and hey, I'm just a hooman after all! 

Besides all, they were impressed with my ```Python```, ```SQL``` and ```Tableau``` knowledge even if they outlined that those skills are "optional" but they would be happy if one knows them very well. 

Thanks to the company and their Data Lead for finding time to explain me what kind of mistakes I was making! 

The thing that I'm mostly proud of is my overall thinkering and analytical abillities, using different libraries for solving the problem and abillity to learn and apply something new on the fly! 

If you are interested how I used ```Tableau``` to answer these questions follow the link provided in the ```tableau-public.txt```. I know it's not super tidy and definetly needs improvements but I was not planning to finish the tasks after being complete perfectionist. I use Pareto principle. ;) 

In the ```data-preparation.ipynb``` you can find how I transformed raw data from Kaggle and joined ```csv``` and ```JSON``` files into one big table that will be useful for solving and visualizing all the outlined challenges, except for the last one which in my opinion is (and was) only ```SQL``` based. Take a look into the ```final-task-update.ipynb``` for the solution. 

Here are some things I've missed:

```

If a video was trending for three days and had 1000 new views every day, and our dataset is:

01.01 1000 views

02.01 2000 views

03.01 3000 views

we cannot just add 1000 + 2000 + 3000 to find the total number of views.

```

and

```
Videos that appeared in multiple countries to determine the behavior of people in those countries.

if our dataset is:

01.01 US 1000 views 101 likes

01.01 CA 1000 views 101 likes

02.01 US 2000 views 202 likes

02.01 CA 2000 views 202 likes

03.01 CA 2500 views 203 likes

it is not necessary that the US and CA like-to-view ratios are ~10%. It can be 20% for the US and 0.2% for CA."
```

I'm going to fix them in the ```data-preparation-v2.ipynb```, and also focus on using ```PySpark``` this time for ```SQL``` tasks, even if it sounds like an overkill for few hounderd rows. 
