# surfs_up
VS Code, Jupyter Notebook, SQL, Python

## Overview of surfs_up

#### This analysis was performed to use SQLAlchemy to query SQLite databases inside of Jupyter Notebook using Python. While it might seem redundant to not just use a SQL program to query SQL databases using the SQL language, this technology allows for more versatility in data analysis using a different medium and allows it to be viewed in different ways. Compared to SQL being limited to tables, the power of Jupyter Notebook and Pandas allows for databases to be converted into DataFrames and visual plots, which diversifies the way the data can be displayed, as well as the functions performed with said data.

#### The climate_analysis file simulates querying weather databases collected for "Awahoo, Hawaii" to gather investors for a "Surf and Shake shop shop serving surfboards and ice cream to locals, tourists, and of course, yourself". The investor, W. Avy, is interested in the idea, but needs easily readable information on the year-round weather (precipitation, temperature), which, using recently acquired knowledge of the languages, programs, and technologies referenced earlier, will be as easy as laying back on the beach.

#### The SurfsUp_Challenge file serves a similar purpose, however done mostly independently. The object of this challenge was to create DataFrames of temperatures for the area during June and December specifically.

## Results

#### There are three notable differences between the June and December temperatures of Awahoo, however similar as they are.

![June](https://i.gyazo.com/559b6b85eacde241e81c6536591039db.png)
![December](https://i.gyazo.com/c0dc934861c08e638bd7a2e5d888eefb.png)

- The average (mean) temperature in June (rounded up to 75°F) is just a bit higher than it is in December (rounded down to 71°F).

- The standard deviation (std) is a higher number in December than it is in June, showing that temperatures fluctuate a bit more between days in December.

- The recorded minimum temperature (min) of all June months provided with the data is 64°F, compared to 56°F for December. On the inverse, the maximum (max) for June was 85°F, and 83°F for December.

## Summary

#### In essence, the temperatures in Awahoo from what's considered a peak summer month (June), to a peak winter month (December), is not drastically different compared to a lot of other places in the world. It doesn't get too hot, and it doesn't get too cold, generally speaking. 

#### While a broad statement, in my opinion this is a very comfortable place to be outside and active, leading to the conclusion that a "Surf and Shake" shop can be considered a good investment for the climate.

![JuneDec](https://i.gyazo.com/79038160644a799318ec75bbcf8298cf.png)

Two more queries that can be involved to get even more specific information on June and December, given that precipitation is another weather variable. While already done broadly in the first file I referenced, it's as simple as changing a bit of the code.

The picture shown above illustrates the difference between the code used to query the precipitation/temperature data for the two months. Changing ***tobs*** to ***prcp*** simply changes the data being filtered.

![JuneDec1](https://i.gyazo.com/f6f186106fd6536cafa4a3f9a78bced3.png)

With code to convert the lists of dates/precipitation scores for June and December into DataFrames, it is now easy to see the differences in rainfall for the two months as well. Had the SQLite file had any other recorded weather data, it would be all as simple enough to record that data as well.
