# COVID19_TimeSeries
Time Series analyses on the COVID19 Dataset provided by Johns Hopkins University

#### Study By
#### JD Kim - Muriel Kosaka -  Gabe Arnold


[Understanding Data](#understanding)


[Models Used](#models_used)


[Final Model](#final_model)


[Model Forecasts](#model_forecasts)


[Recommendations](#recommendations)


<h3 name='understanding'>Understanding Our Data</h3>

![COVID-19 Cases](./Images/Cases_Over_time.png)

[JHU GitHub](https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data) 

<p>
Our dataset was collected from JHU GitHub. It contains up-to-date information regarding the latest number of COVID-19 confirmed cases and COVID-19 Deaths. Although these models were only ran on domestic (United States) data, international data is also available.
</p>

[Google Slides Presentation](https://docs.google.com/presentation/d/19bSeF2CYUXwHmU5_qNF629tYyzYrAgu9pLZPx3qws1M/edit?usp=sharing)


<p>
Since the beginnning of the year, COVID-19, has spread across the entire world at an alarming rate. The first case in the United States was recorded in January 2020. As of July 30, 2020 millions of people have been infected, and over 150,000 people in the US, have died from the virus. We wanted to see if we could build a model to see where the numbers are heading.
</p>

<p>
Our goal is to build a model to project death and confirmation rates on a state and national level in America. Also see if certain actions can be made to decrease the rate of the curve.
</p>

<h3 name='models_used'>Models Used</h3>
    
<ul>
    <li>ARMA</li>    
    <li>ARIMA</li>
    <li>SARIMAX</li>
</ul>

<h6 name = 'final_model'>Final Model</h6>

<p>
The final model selected was SARIMAX model. The RMSE Score for the National Cases Confirmed model was 15,325. The RMSE Score for the National Death Model was 487.
</p>

<h3 name='findings>Findings</h3>

<h6>Confirmed Cases </h6>

<p>
Highly populated areas were hit extremely hard. We believe that it is a result of the dense population and high transmission rates. New York City and Cook County (Chicago), had large jumps in the number of people that were initially infected during the lockdown phase, however, data shows a smoothing in the recent rate of cases, even after reopening. It should also be noted that both of these cities instituted a lockdown relatively early and longer in the US.
</p>

![Cook County/Chicago Confirmed Cases](./graphs/chicago_confimed.png)
    
<p>
Recently, the counties of Los Angeles County, California, Harris County, Texas (Dallas), and Maricopa, Arizona (Phoenix), have seen large increases in the number of people that have recently contracted the disease. Los Angeles, even though they instituted a longer lockdown compared to other cities in America, has faced a rapid increase in the number of confirmed cases. Harris County, Texas and Maricopa, Arizona had shorter lockdown periods and are now experiencing a rapid increase in cases after reopening.
</p>

![Phoenix Metro](./graphs/phoenix.png)

![Harris County, Texas](./graphs/harris_county.png)

<p>
Additionally, we noticed in median populated (~12,000 People) regions, that had shorter lockdown periods are experiencing high rates of infection.
</p>

<p>Areas with small populations (Less than 1,000 People), face small amounts of Contamination Cases.</p>

<p>In large (>4,000,000) and median populated regions generally saw a spike after the Fourth of July.</p>

<h6>Death Cases</h6>

<p>
Death cases were similar to confirmed cases. Large metropolitans that were hit early experienced very high death rates. As we transition to overall state data, we can see New York, California, and Massachusetts are all leading the nation in COVID-19 deaths. 
</p>
    
![US Death Count](./graphs/top_10_states.png)

<h3 name='model_forecasts'>Model Forecasts</h3>

<p>Currently, our models predicted that there will be a continuation of the upward trends in both confirmed cases and death cases, however the amount varied depending on the location. </p>

![Mass State Forecast](./Images/Massachusetts_Death_Cases_Forecast.png)

![New York City Confirmed Cases](./Images/New_York_Confirmed_Cases_Forecast.png)

![California State Confirmed Cases](./Images/California_Confirmed_Cases_Forecast.png)

<h3 name='recommendations'>Recommendations</h3>

<p>
Based on the analysis performed, it is recommended that cities institute some measure of lockdown protocol. As this has shown promise in mitigating the cases and and keeping the death rate down.
</p>

