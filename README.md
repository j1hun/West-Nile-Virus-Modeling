# West-Nile-Virus-Modeling

### __Introduction__

West Nile virus (WNV) is the leading cause of mosquito-borne illness in the United States. Between 1999 and 2019, over 7 million human cases were reported with over 50,000 severe cases of West Nile fever and 2400 fatalities. Forecasting when and where WNV outbreaks might occur is an essential task for mosquito control programs.

To monitor for infections, mosquito control program maintain and monitor many different mosquito traps in their district. For instance, the city of Chicago maintains several hundred traps all over the city. Each day workers test these traps by counting the number of mosquitos and testing if any mosquitos are WNV positive. Finding a large number of traps with WNV positive mosquitos means that the local population is at severe risk of WNV infection.

### __Background__

Waiting for traps to test positive means that it will be too late to take preventative action. Instead, Mosquito control programs use statistical methods to forecast if an outbreak of WNV is likely in the next several days. These models use historical outbreak information, spatial information, climate variables, and demographic data to help predict when and where WNV is likely to occur. 


### __Task__

Our task is to build a forecasting model to predict the prevelance of WNV across Chicago one, two, and three weeks in advance

We will model the average _minimum infection rate_ (MIR) each week at each trap location. The MIR is defined as


$$
\text{MIR} = 1000 \times \frac{\text{number of positive traps}}{\text{number of mosquitos tested}}
$$


For example, if we tested a trap 5 times during the week and saw 10 mosquitos each time and 3 times the trap was positive then $\text{MIR} = 1000 (3/50) = 60$.

We need to build a regression model(s) to predict $$MIR_t, MIR_{t+1}, MIR_{t+2}$$ based historical information and other covariate information. 


