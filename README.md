<h1>COVID-19 Pandemic and the Role of Vaccinations
<br>A Cross-Country Comparative Analysis</h1>

<h2>Introduction:</h2>
<p>The COVID-19 pandemic has been at the forefront of international news, affecting all countries with differing levels of severity. The following analysis presents the brief overview of the global pandemic and vaccination progress. In order to maintain a balanced and objective evaluation, the focus was put on two economically contrasting countries, the United Kingdom and Kenya. The in-depth comparison investigates which country turned out to be more affected by COVID-19 and which response was more effective.</p>

<h2>Abstract</h2>
The following git hub repository contains following files:
<ul>
<li>Data folder – with 2 datasets (country_vaccinations.csv, worldometer_coronavirus_daily_data.csv)</li>
<li>Output folder – containing relevant summary data frames for global overview, vaccination and country specific information</li>
<li>Images folder – containing all of the visualisations included in the analysis</li>
<li>5 Jupyter Notebooks containing data analytics for global overview, vaccination summary, combined UK and Kenya analysis and country specific analysis</li>
<li>Presentation file – slide deck containing analysis visuals and summary</li>
<li>Requirements.txt – document containing the list of the python libraries used throughout the analysis</li>
</ul>

<h2>Methodology</h2>
<p>The analysis was conducted fully using Python and was based on two datasets – ‘Country Vaccination’ and ‘Worldometer Coronavirus Daily Data’. During the analysis some of the datasets’ limitations and disparities were identified. The first dataset splits the United Kingdom into constituent countries and provides specific data for each of them. To maintain the precision and relevancy of the comparison, some manipulation was necessary. A separate data frame was created for each country and then merged on date to create a combined dataset for the United Kingdom with the ability to still view the change over time. 
A variety of Python libraries was used throughout the project. Most of the work was done using Pandas, Matpolotlib and Geopandas. The Pandas library was used for displaying and cleaning the dataset, identifying and pulling out relevant data, creating new data frames and merging the existing ones. Once the summary statistics were generated, the visualisations were created using Matplotlib and Geopandas.</p>
<h2>Results</h2>
<h3>Global Overview</h3>
<h4>Is COVID-19 a deadly disease? Would it be an infectious disease in a short-time period? </h4>
<img src=https://github.com/DominikaRzez/Project1_CovidVaccinationAnalysis/blob/main/images/Correlations.png?raw=true>
<small>Figure 1 Correlations between total cases and total deaths</small>
<br>
<br><p>As presented in figure 1, COVID-19 has shown to be a deadly disease with a strong correlation between confirmed cases and total deaths. Moreover, it has also demonstrated to be a fast-killing virus showing a stronger positive linear correlation in shifting 7 and 14 days confirmed cases than in shifting 1 day or 30 days as seen in figure 2.</p>
<img src=https://github.com/DominikaRzez/Project1_CovidVaccinationAnalysis/blob/main/images/dynamic_correlations.png?raw=true>
<small>Figure 2 Correlations in dynamics</small>
<br>
<br><h4>How infectious is COVID-19? Are our econometric results statistically significant?</h4>
<img src=https://github.com/DominikaRzez/Project1_CovidVaccinationAnalysis/blob/main/images/Regression1.png?raw=true>
<small>Figure 3 Linear regression between daily cases in 7days and daily deaths</small>
<br>
<br><p>According to the regression analysis results displayed in figure 2, each confirmed case can cause between 8 to 9 deaths after 7 days or around 12 deaths after 14 days. The T-test shows the p-value is less than 0.005 suggesting population sample of case confirmed and population of death are different groups of dataset statistically. With Adjust R-square value equal approximately 0.73 and 0.57 for two regressions in slides 10, we find that COVID-19 case to be confirmed 7 or 14 days ago may explain 73% or 57% of the reason for people’s death afterwards.</p>
<h4>Which countries are the most efficient in distributing the COVID vaccination programme?</h4>
<img src=https://github.com/DominikaRzez/Project1_CovidVaccinationAnalysis/blob/main/images/share%20of%20people%20fully%20vaccinated_map.png?raw=true>
<small>Figure 4 Choropleth map of percentage of population fully vaccinated across the world</small>
<br>
<br><p>Further analysis was conducted for global vaccination progress and a choropleth map was plotted as displayed in figure 4. An evaluation was provided for percentage of the population vaccinated in each country rather than number of people as this allows a more significant comparison.
The data showed that vaccination distribution differed across the world. Figure 4 presents global share of people fully vaccinated by June 2021. The highest rate of vaccination was observed within small islands and countries like Gibraltar, San Marino or Malta. Of the larger countries, the United Kingdom had a high rate of vaccination with almost 50% of the population being fully vaccinated at the time data was collected. Similar vaccination rates were observed for the United States, Hungary and Chile.
Towards the lower end of the vaccination rate global rankings, a large proportion consisted of mostly African countries alongside a few Middle Eastern countries. The majority of these nations had approximately only 1% or less of their respective populations vaccinated.

<br>Based on these disparities, further analysis was conducted for two contrasting countries – the UK as the leader of the vaccination programme and Kenya as the slower distributor of the vaccine.</p>
<h4>UK and Kenya comparison</h4>
<img src=https://github.com/DominikaRzez/Project1_CovidVaccinationAnalysis/blob/main/images/uk_vs_kenya_population.png?raw=true>
<small>Figure 5 Population difference in Kenya & UK</small>
<br>
<br><p>From figure 5, the UK population was 68.39 million in comparison to Kenya’s 55.45 million. The UK has a greater population with a percentage difference of 20.9% between the two countries. Due to this, it is possible that the UK will have more confirmed cases. As COVID-19 is a viral disease, it is transmitted between people through respiratory particles. Therefore, if the population of the UK is greater and Kenya is 2.4 times bigger than the UK, that would mean more people are in close proximity within the UK in comparison to Kenya. Ultimately, the probability of catching COVID in the UK is greater.</p>
<h4>How did the UK do during the COVID-19 pandemic from March 2020 to November 2021? </h4>
<img src=https://github.com/DominikaRzez/Project1_CovidVaccinationAnalysis/blob/main/images/UK_daily_cases.png?raw=true>
<small>Figure 6 Daily new cases in UK from March 2020 to November 2021</small>
<br>
<br><p>The UK has been the most impacted country, following the USA, India and Brazil. As displayed in figure 6 the UK identified 5000 new COVID-19 cases corresponding with 650 deaths in figure 7. It was during this period where the government announced the first national lockdown. The lockdown had a positive impact as the numbers of new covid cases declined and stayed steady until May 2020, with daily new cases going down to 1500 with corresponding deaths of 60. It was on this basis that the PM announced the easing of restrictions.</p>
<img src=https://github.com/DominikaRzez/Project1_CovidVaccinationAnalysis/blob/main/images/UK_daily_deaths.png?raw=true>
<small>Figure 7 Daily new deaths in UK from March 2020 to November 2021</small>
<br>
<br><p>Unfortunately, cases and death numbers gradually inclined between months October 2020 to December 2020, as evident by the steep progress in figures 6 and 7. A top record of daily cases topped 54000 in January 2021 and deaths peaking to 1000!
The panic squandered within the public and it was January 2021 where the PM announced the second national lockdown in the UK. The national lockdown massively helped with the new numbers of daily cases decreasing to 2000 in April 2021. Alongside this the contributions of the vaccines also helped with 200,000 daily vaccinations being rolled out in January 2021 alone as shown as a peak in figure 8.</p>
<img src=https://github.com/DominikaRzez/Project1_CovidVaccinationAnalysis/blob/main/images/daily_vaccination_by_country.png?raw=true>
<small>Figure 8. Daily vaccinations by country</small>
<br>
<br><h4>How did the Kenya do during the COVID-19 pandemic from March 2020 to November 2021? </h4>
<img src=https://github.com/DominikaRzez/Project1_CovidVaccinationAnalysis/blob/main/images/kenya_daily_cases.png?raw=true>
<small>Figure 9 New COVID-19 cases in Kenya from March 2020 to November 2021</small>
<br>
<br><p>Figure 9 displays a timeline of daily new COVID-19 cases in Kenya from March 2020 to November 2021. The line graph shows 4 significant peaks where the number of new COVID cases were at their highest; the highest being on 1st April 2021 which had recorded 984 new cases in the country. The lowest number of daily cases recorded was on 27 November 2021 with a value of 36 new cases.  The non-monotonic pattern of the daily new cases across the timeline may be due to extraneous variables such as the number of different strains that were discovered during the pandemic. In addition, travel, social distancing and implemented measures such as lockdown and curfews were different across the globe. This may have influenced the results obtained.</p>
<img src=https://github.com/DominikaRzez/Project1_CovidVaccinationAnalysis/blob/main/images/kenya_daily_deaths.png?raw=true>
<small>Figure 10. New COVID-19 deaths in Kenya from March 2020 to November 2021</small>
<br>
<br><p>As displayed in figure 10, the highest number of daily new deaths was 20 on 1 May 2021 and the lowest being on 27 November 2021 where there were 0 deaths recorded in the country. In relation to the daily new cases, both graphs had the least number of cases and deaths towards the backend of 2021. This may be due to the increased number of people taking vaccinations, flight restrictions for travellers that enter the country to prevent further spread as well as regulations within the country. Regarding the highest peaks in both figures, it could be deduced that out of the 984 new cases on 1st April 2021, 2.03% of those that tested positive could have led to fatality.</p>
<h4>Which country was affected more during the pandemic?</h4>
<img src=https://github.com/DominikaRzez/Project1_CovidVaccinationAnalysis/blob/main/images/COVID_in_kenya.png?raw=true>
<small>Figure 11. COVID-19 in Kenya</small>
<br>
<br>
<img src=https://github.com/DominikaRzez/Project1_CovidVaccinationAnalysis/blob/main/images/COVID_in_uk.png?raw=true>
<small>Figure 12. COVID-19 in UK</small>
<br>
<br><p>Kenya had 0.46% total confirmed cases out of the population, with only 0.01% of those caused fatalities. The total recovery out of those with confirmed cases concluded to be 97.28%. This shows that during the initial stages of the outbreak, Kenya was not affected as much. Whereas for the UK, the total number of confirmed cases was 15.18% of the population. This is significantly greater than that of Kenya thus showing that the UK was affected more by the pandemic. Although the total number of confirmed cases is high, the total number of those that recovered out of the confirmed cases turned out to be 88.21%. The number of active cases in the UK was 1.58% compared to Kenya’s 0.003%. These findings support the hypothesis. These calculations can be interpreted as Kenya having more control of the coronavirus than the UK. However, the population difference may suggest that because the UK has a greater population than Kenya, the spread of COVID will be amplified.</p>
<br>To summarise, Covid-19 has proven to be a fast-killing virus globally however with the intervention of vaccinations ongoing figures show a successful slow of infections and deaths which has been demonstrated in countries like the UK and Kenya.

<br><i>Further in-depth comparison within the UK and Kenya and visualisations can be found within the images folder and Jupyter Notebook.</i></p>



