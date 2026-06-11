
Climate Change Analysis: Emissions, Energy, and Temperature Trends

Introduction :
Climate change is one of the most pressing challenges of our time, yet the 
relationships between its key drivers are not always easy to see in raw data. 
This project set out to answer a straightforward question: can we use publicly 
available climate data to clearly demonstrate the connections between human CO2 
emissions, shifts in global energy consumption, carbon market behavior, and 
rising temperatures — and can we build models that project where these trends 
are heading?

The motivation behind this work was to move beyond headlines and look directly 
at the numbers. While the scientific consensus on climate change is well 
established, we wanted to understand the data ourselves, visualize it clearly, 
and apply machine learning to see how well historical patterns can predict 
future outcomes.


We worked with five real-world datasets covering the period 2000 to 2026, 
including yearly CO2 emissions by country, monthly global temperature anomalies, 
national energy mix breakdowns, daily EU carbon market prices, and a timeline 
of major climate events and policy decisions.

The work was carried out in five stages. We began by loading and cleaning all 
five datasets — handling missing values, correcting data types, and preparing 
unified tables for analysis. In the second stage we built a series of 
visualizations to explore the data: temperature trends over time, CO2 emissions 
by country, the global shift in energy sources, and the relationship between 
atmospheric CO2 concentration and surface temperature. The third stage produced 
a multi-panel dashboard that overlaid real climate events — heatwaves, disasters, 
and policy milestones — directly onto the temperature and carbon price timelines, 
making it possible to see how real world events left measurable signals in the data.

The fourth and fifth stages focused on predictive modeling. We built two separate 
machine learning models using Linear Regression and Random Forest algorithms. The 
first model forecasts global CO2 emissions through to 2050 based on historical 
trends. The second predicts monthly temperature anomaly using atmospheric CO2 
concentration and emissions data as inputs. Both models were evaluated using 
standard metrics including Mean Absolute Error and R-squared score. In both cases 
Random Forest outperformed Linear Regression, and the temperature model in 
particular demonstrated a strong and consistent relationship between CO2 levels 
and surface warming.

The results confirmed several patterns worth noting. Global temperatures have 
risen by approximately 1.0 degree Celsius above the 1951 to 1980 baseline, with 
the rate of increase accelerating after 2000. China and the United States 
dominate total emissions, though per capita figures tell a more nuanced story. 
Renewable energy has grown meaningfully across all regions but fossil fuels 
remain dominant globally as of 2023. EU carbon prices were largely flat until 
2018 and then rose sharply following stronger policy commitments, a shift that 
is clearly visible when prices are plotted against the policy events timeline.

---

Conclusion :

This project demonstrated that publicly available climate data, when properly 
cleaned and analyzed, tells a coherent and concerning story. The connections 
between CO2 emissions, atmospheric concentration, and temperature rise are not 
just statistically significant — they are visually obvious once the data is 
presented clearly.

From a technical standpoint, the project showed that machine learning models 
trained on historical climate data can produce reliable short to medium term 
forecasts, though they cannot account for future policy changes or technological 
breakthroughs that may alter current trajectories. This is an important 
limitation shared by virtually all climate forecasting models.

Looking ahead, this work could be extended in several meaningful directions: 
incorporating real time data updates through public APIs, expanding the carbon 
market analysis beyond the EU, and building an interactive web dashboard that 
allows users to explore the data themselves. A deeper modeling approach using 
neural networks could also improve forecast accuracy over longer time horizons.

Ultimately this project reinforced for us that data science is not just a 
technical exercise. Applied to a topic like climate change, it becomes a tool 
for understanding the world more clearly and communicating that understanding 
to others.