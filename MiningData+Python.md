# Maximizing Iron Concentration: An Insightful Analysis with Python

Dive into the world of mining data analysis with me. As a newly hired data analyst for Metals R' Us, I was tasked with analyzing real data from their flotation plant from March 2017 to September 2017 and focus on the iron concentration.  

The way the process works is first the iron ore goes through a flotation process to become cleaner. Then the ore is mixed with starch and amine to remove dirt, and last the air bubbles are added to separate the iron and minerals. The process happens in three steps.

Containing columns sampled every 20 seconds and others every hour, I uncovered insights about the purity of iron concentrate using a comprehensive toolkit of Python, Pandas, print statements, mathematical operations, functions, loops, and data visualization. Join me as I share my findings and demonstrate the power of data analysis.

<a href="https://www.kaggle.com/datasets/edumagalhaes/quality-prediction-in-a-mining-process?resource=download">THE DATA</a>

## PREPARING THE DATA 
### Import necessary libraries: pandas, matplotlib, seaborn, and fix the format issues (comma to decimal)
IMAGE HERE

### Load the data into a pandas dataframe
IMAGE HERE

### Quick look of the data size, changed a str to a date
IMAGE HERE 
I needed a quick understanding of the size and type of my data columns, date went from str to a datetime type as I needed it for my visualizations over time later on

IMAGE HERE
Using one line of code I got a great overview of the data statistics such as the min, count, max, and average values


# ANALYSIS 

### Plot the distribution of % Iron Concentrate using histogram
IMAGE HERE 

A bimodal left-skewed distribution of % Iron Concentrate suggests two groups with different quality levels, with most samples having lower quality. The higher peak may indicate higher quality and the lower peak lower quality. Further analysis is needed to gain deeper insights
IMAGE HERE

### Plot a line chart to show the changes in % Iron Concentrate over time

IMAGE HERE 
A line chart showing % Iron Concentrate vs. time didn't show any significant trends, implying that factors like production process, raw materials, and environment don't greatly affect iron concentrate quality.

### Line charts of all the important columns
IMAGE HERE
Creating line charts for important variables can help understand the relationship between variables and identify trends in the data, including the % Iron Concentrate in a mining floating plant. This can help identify correlations and find factors that significantly affect the quality of the iron concentrate.

### Conclusion

The analysis shows that the % Iron Concentrate increases between 4 AM – 6 AM and 7 PM – 9 PM, while Silica Concentrate decreases during these times. There appears to be a relationship between Iron Concentrate and Silica Concentrate, with an increase in Iron Concentrate resulting in a decrease in Silica Concentrate. Ore Pulp Flow and Amina Flow also seem to be related, as they both increase when Silica Concentrate is at its lowest. This suggests that the usage of Amina, a reagent used to separate silica from iron ore, is likely affecting the concentration of silica, Ore Pulp Flow and Amina Flow.

The observed relationship between Iron Concentrate, Silica Concentrate, Ore Pulp Flow, and Amina Flow is likely due to the usage of Amina as a reagent. An increase in Amina usage decreases silica and increases Ore Pulp Flow and Amina Flow.
