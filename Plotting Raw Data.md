# My Thought Process in Plotting Raw Data for Clean Sydney Beaches
Please refer to my [Plotting Raw Data script](https://github.com/cathybiocodes/RYouWithMe/blob/main/Plotting%20Raw%20Data) to see what I used to code these plots. Data used from Sydney Clean Beaches provided by RLadiesSydney.
This first graph I made with geom_point, but the observation points are on top of one another. 

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/c22aed57-3820-4db4-8595-cbbab93dc93d" />

To get a better view of the data I need, I used geom_jitter for the next plot. Honestly, a lot better to look at the number of observations of this data set.
However, I also needed to omit some rows in my data for better accuracy. 

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/fb0128aa-2160-4200-ad66-504d6f160ffd" />

The sites were also not as readable so I flipped the coordinates. It is starting to look better with my coordinates flipped. 

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/c7b8223e-0545-466b-8a69-af24f37b7d2b" />

Adding color would help view the different years, but the data recognized my 'year' variable as a sort of integer instead of a factor, so it made the colors scale.

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/97ae9665-1810-4dbd-a7ea-e7c374d73174" />

I changed that by making the 'year' into a factor and reran the code to get another plot.

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/a46274b9-e008-4a0d-b87b-cc6f2da4a2a8" />

The plot still had a lot of overlapping data, which made it hard to differentiate the data by variables. I then used facet_wrap to make smaller graphs for each site.

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/69c327e0-a049-482e-adb5-cd80fbe92f91" />

Looking at the plot, the scale was off by some outliers. I changed the scale to up to 1000 to reflect the majority of the data in the set. 

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/2f073caa-3293-4996-b347-adeeb5f59f6b" />

It looks so much prettier. I was also curious about certain sites, so I filtered further for Coogee Beach and Bondi Beach. 

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/d947c42c-2d1e-4fef-bf9b-92a4e567e145" />

It was interesting to see how clean the different beach sites have gotten over the years. Above shows my thought process in playing around with ggplot and dplyr packages
with this tutorial provided by RLadiesSydney. It was a great refresher and different from other R modules that I have followed.



Following along the tutorial to learn more visualizing different types of boxplots, first I plotted a very basic boxplot but I want it to be prettier.

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/3e0cda6d-32c6-4e8e-818a-f982d2834447" />

I learned how to use the violin plot from ggplot2 and got a basic one to show first

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/ba36e329-d1b7-4630-a7e7-d555bdc49cac" />

Then I filtered the data by site with a facet wrap

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/4b9334be-c609-455d-b1d1-32bc898e9e1c" />

Added color with filling by year

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/f3470c8f-d533-4799-ac80-e2b5400b590b" />

Sometimes I just need to look at the data real quick so I used a basic histogram code and adjusted the spacing

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/b79cd347-3faa-4158-9868-b2c24cced4e6" />

Took everything I learned so far from and combined them all into a boxplot

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/f16ffe1c-c731-4452-9c6a-9216e7c0ac42" />

Then I wanted to see what it would look like in a violin plot with the points scattered in the filling

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/4ec38327-2fa2-493e-a2ba-0bf08573a93f" />

Overall, it was more fun learning the violin plots. The thinner sides show off the outliers and it is just visually more appealing. 

Trying out bar plots with this dataset so I could get the basics and the build on top of it. I used geom bar so that R could automatically give me a count of my observations.

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/36cb5f8d-b5a5-448f-a5fd-34d1b0273167" />

In this one i used geom col so that I could define the variable on my y axis, so that the height of my bars shows the values

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/db3ae327-4d06-48b8-bd0a-1271a2bb0091" />

I also wanted to include error bars. I flipped the coordinates in this one for easier readability

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/fa74067d-2a9f-4916-8df2-75b83083161a" />

Please refer to my raw data script to find another data set that I used to get this next graph. I wanted to get a correlation plot using scatterplots and a regression line with some color.

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/bf96ed6d-a285-4326-95d4-d0aa4d38c249" />

Definitely getting better with my graphing skills here at this point, but would the table be something I could present? This next one I was playing around with the themes available and got rid of the gridlines. 

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/cbd7c42e-6870-4f9c-9d95-30494b1904bf" />

Then I loaded another package called RColorBrewer and played with the colors some more.

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/b986e7c0-6211-47e4-aa12-d0e9e35fb91b" />

I did need to look at some of the palettes available in the package so I displayed it for easy viewing, before putting the color gradient in my script.

<img width="1227" height="752" alt="image" src="https://github.com/user-attachments/assets/efd2e727-51a4-4a99-a32a-b7628d42a10a" />

I picked a color gradient to show a continuous change in temperature in this graph, from blue to red as the heat goes up.

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/618f0f6e-575c-4140-b191-d6ff5f0bc05b" />

Then I put on the proper aspects for a graph that could be presented at a conference, such as title, labels, and data source.

<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/b9255707-0b52-4812-b167-f356905d8cb1" />

There is certainly a lot that could be done with different color aspects, and I have not even touched half of the ggplot package yet.

There is so much that could be done with ggplot and I dont even know the half of it. Had fun adding a gif to a plot, but the file is too big for me to add here. 










