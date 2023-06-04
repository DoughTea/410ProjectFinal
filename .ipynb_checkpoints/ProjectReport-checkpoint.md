# Introduction
I have been a fan of Porsches for most of my life. I have grown up wanting one and while the day where I will actaully get one is still far I want to prepare. In this preperation I wanted to look at the prices for the different models and years. The initial goal was to see how the number and price of listing has changed over the years. However, I ran into some problems that I will get into later that led me to change the question to "When do automatic transmissions become more expensive than manuals?".
## Modivation
### Why are you planning to do this analysis?
I am planning to do this analysis because I want to know if I will ever be able to afford a Porsche. While I don't want to say that it is my dream, I do hope to own one in the far future.

### Why is it potentially interesting and useful, from a scientific, practical, and/or human-centered perspective?
I think that this will be interesting. I want to looking when it became cheaper to get an automatic vs a manual. I want to look into the number being listed over time vs the price. To see if less are being posted and the proces are going but (very bad for me). This research could help others see if they too will every be able to get a Porsche in the future. I think that the research could also be transfered to other cars if poeple wanted to copy my methods and look into a different one.

### What do you hope to learn?
I hope to learn that the price is not changing too much when considering inflation and that there is still a healthy amount being sold. Even better would be if the price was going down. But academically I hope to improve my open research process, getting better at leaving notes on what I am doing and why. I also want to improve my data analysis skills.

# Background & Related Work
I have done similar research for another class that looked at all the cars on craigslist. So I already have an idea to what data is included and some general trends. While this report does not focus on it, it was interesting to see how Porsches statistics compare to the rest.

## Data

### What dataset do you plan to use, and why?¶
I plan to use a data set from craiglist about car listings in the United States. I am choosing it because it is hard to get your hands on large car selling information for free and so I chose this one beacause it is large and free. It also contains a bunch of columns that might be helpful for analysis later.

### Summarize what is represented in the dataset
It has 426,881 rows and 26 columns of data. It is from all of the United States. While I can't use all of it since I am only focusing on Porsches, it should have enough rows of them to be usable. If it does not then I will have to switch projects. It has these url, region, region_url, price, year, manufacturer, model, condition, cylinders, fuel, odometer, title_status, transmission, VIN, drive, size, type, paint_color, image_url, description, county, state, lat, long, posting_date.

### Link to the dataset (it must be publicly available)
https://www.kaggle.com/datasets/austinreese/craigslist-carstrucks-data

### Specify license and/or terms of use for the data
CC0: Public Domain

### Explain why this dataset is a suitable one for addressing your research goal listed above
It should have all the nessary variables that I need to find out relationships. It also is large enough where I should have enough data to look at and graph.

# Research questions & hypotheses

## Reseach Question
When do automatic transmissions become more expensive than manuals?

## Hypothesis
I think that it will be around the mid 2000's. This is because that is when they started to get really good. Before this the automatics were fine but were not that much better than a manual. After this time however the automatics they were making became very fast and better in almost every way.

# Methodology

## First Steps
After I downloaded the data from the website I needed to sort through it to get all the Porsches. 

## Cleaning the data
I used a SQLite3 to create a new table. I then wrote a quarry to filter through the data. You can download the SQL table here. It is the carData file. 
The Quarry I used was something like "sqlite3 -header -csv my_db.db "SELECT * FROM carData car WHERE "manufacturer" = "porsche";" > porsches.csv"
From there I just cleaned the data within tableau. This just looked like removing null values and setting minimuns for the count.

## Changing topics
As I was looking at the data I realized that it was really just collected over a year, so doing an over time evaluation was going to be impossible. That is why I ended up switching my project focus into the transmission since that was something I was also interested in. It was also something that I could do without finding a new dataset which is what I wanted to avoid since finding one is very annoying.

## Vizualizing the data
Deciding what I was going to vizualize was mostly going off my gut. I have been looking into cars for a while so I kinda had an idea what I wanted to look at. Since I can only focus on so much I first wanted to only look at my favorite the Porsche 928, pre 1987 to be exact, but there were less than 10 which is not super helpful. So instead I decided to look at transmissions since those are also a pretty fun area of cars. At first I put it into tableau to generate some of the visualizations, which are in the visualizations folder here. Then the altair visualizations are in the AltairGraph ipynb. I wanted to make a box and wiskers graph for the price over the years for manual vs automatic. 

## Presentation
Graphs are going to be my friend here. Showing the average price by year for each in a bar chart would be effective. A QQ-plot would also be great for this situation. But unless chat gpt can walk me through it in tableau then I will not do it since I HATE R which is where my QQ-plot graph code is.

## Why
These methods make sense for me since I know how to do them and they would be useful in finding the relationship. They would show how the price changes over time and it would be easy to compare.

# Findings
Can't really draw any conclusions from the data that I had. There is just not enough of it. The price of automatics does start to rise in the late 2000's but that could be attributed to the cars just being newer. It is also unlucky because after 2010 we don't see a lot of manuals. This could be an indicator that they were less desirable then so less people got them. But again it is hard to be certain of any conclusions without more data.

# Discussion (including Limitations and Implications)
The largest limitation was the data itself. It is very hard to get good car data for free. The people who collect it do so to sell it and so since I didn't want to pay for data that made it tough for me. 
I also do not have the best statistical analysis knowledge. In this case I think that it was fine because looking at the graph it looks like there is not enough data to do one in the years that I want.
The implication of this is that I don't have statistical analysis to truely back up my claim. But this is fine since my conclusion is that there is no conclusion.

# Conclusion
I am very happy that I chose this to be my topic. It was interesting to look at and while I did not get conclusive results I still learned a lot. I will continue to use this data source to look at the prices. I will also use the tools that I got good at during this research to continue to try and find a trend. The next steps for this are finding better data for starting to collect my own. I have been meaning to start collecting my own so this might be my sign to start. 