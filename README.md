# 410ProjectProposal
# Summary
<<<<<<< HEAD
This looking into the price of different Porsches and what facotors effect price. The goal of  this research is to find out if I can own one many years from now. This research looks for trends that might suggest that I will not be able to.

# First Steps
After I downloaded the data from the website I needed to sort through it to get all the Porsches. 

# Cleaning the data
I used a SQLite3 to create a new table. I then wrote a quarry to filter through the data. You can download the SQL table here. It is the carData file. 
The Quarry I used was something like "sqlite3 -header -csv my_db.db "SELECT * FROM carData car WHERE "manufacturer" = "porsche";" > porsches.csv"
From there I just cleaned the data within tableau. This just looked like removing null values and setting minimuns for the count.

# Changing topics
As I was looking at the data I realized that it was really just collected over a year, so doing an over time evaluation was going to be impossible. That is why I ended up switching my project focus into the transmission since that was something I was also interested in. It was also something that I could do without finding a new dataset which is what I wanted to avoid since finding one is very annoying.

# Vizualizing the data
Deciding what I was going to vizualize was mostly going off my gut. I have been looking into cars for a while so I kinda had an idea what I wanted to look at. Since I can only focus on so much I first wanted to only look at my favorite the Porsche 928, pre 1987 to be exact, but there were less than 10 which is not super helpful. So instead I decided to look at transmissions since those are also a pretty fun area of cars. At first I put it into tableau to generate some of the visualizations, which are in the visualizations folder here. Then the altair visualizations are in the AltairGraph ipynb.

# Conclusions
Can't really draw any conclusions from the data that I had. There is just not enough of it. The price of automatics does start to rise in the late 2000's but that could be attributed to the cars just being newer.
=======
This looking into the price of different Porsches and what facotors effect price. The goal of  this research is to find out if I can own one many years from now. This research looks for trends that might suggest that I will not be able to.
>>>>>>> ae32a189695328150ea1bfa80d93d398da605056
