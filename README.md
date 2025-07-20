# Statistical Analysis – Women's Cycling Performance
This project explores whether early performance (during the first 5 laps) can predict final outcomes in a women's cycling race. It is based on race data including lap times and positions.

<p align="center">
  <img src="https://th.bing.com/th/id/R.3d3cad0d6ed5b92dde28e57bc1b0ccf6?rik=AXjB4N6KV9KwBQ&pid=ImgRaw&r=0" 
       alt="Women's Cycling" 
       width="400"/>
</p>


## Objective
To determine if the average performance during the first 5 laps can predict the final ranking (at lap 20) of female cyclists.


## Tools Used
- **JASP** – for statistical analyses (correlation and regression)

## Data Used
Two datasets were analyzed:
- `women race position.csv`: Cyclist rankings for laps 1–5 and lap 20.
- `women lap time (secondes).csv`: Lap times in seconds for the same laps.

Key variables:
- `lap1` to `lap5`: position or time on each lap
- `lap20`: final lap position or time
- `avg_lap1_5`: average over laps 1 to 5

## Analyses Performed
### Correlation – Rankings
- **Pearson’s r = 0.535**
- **p < .001** ➜ Statistically significant
- **Interpretation**: Cyclists with strong early rankings tend to finish higher.

### Linear Regression – Rankings
- **R² = 0.286** ➜ 28.6% of variance explained
- **p < .001** ➜ Model is significant
- **B = 0.548**
- **Conclusion**: Poor early positioning predicts poor final ranking.


### Correlation – Lap Times
- **Pearson’s r = 0.449**
- **p = .007** ➜ Statistically significant
- **Interpretation**: Faster cyclists early on tend to remain faster by the end.

### Linear Regression – Lap Times
- **R² = 0.201** ➜ 20.1% of variance explained
- **p = .007**
- **B = 4.637**
- **Conclusion**: A slow start leads to a slower final time.


## Conclusion
Early race performance is a **reliable predictor** of final outcomes, both in terms of **ranking** and **time**. This finding can inform coaching strategies and race planning.
