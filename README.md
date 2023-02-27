# Student Data Analysis

## Project Overview
Maria seeks analysis on an updated data set of student information do analyze the. Within the dataset we can find the following categories Student ID, Student Name, Grade, School Name, Reading Score, Math Score, School Type. School Budget (See raw data screenshot below)

![Raw_Data_Screenshot](https://github.com/koenesjasmine/Module-4-Pandas/blob/main/Resources/Raw%20Data%20screenshot.PNG)

### Steps taken
> - The data is to be loaded in to python leveraging the pandas library. 
> - drop any null values from the data frame. 
> - drop duplicates from the data
> - convert types as needed to be more in line with intuitive expectations (eg. grade level from "9th"[string] to 9[int])
> - provide summary statistics for the dataset [using .describe()]
> - develop additional analysis and conclusions from the data set

## Data Summary Results
Detailed results can be found at the jupyter notebook at the link below:

[Jupyter School District Notebook](School_District_Analysis.ipynb)


## Conclusion

There are a significant number of null reading (1968) and math scores (982). It may be useful to understand why they are null and perhaps find another method to mitigate rather drop the entire rows (perhaps set them to average or NaN). Based on the data that is available the primary take-aways I saw were that generally the charter schools appeared to have less funding and produce slightly higher reading and math scores, as you can see in results below


|School Type  | Average Budget    | Average Reading Score | Average Math Score  |
|-------------|-------------------|-----------------------|---------------------|
|Public       |   $911,195        |72.281219              |   62.951576         |
|Charter      |   $872,625        |72.450603              |   66.761883         |


However we may need to account for additional variables such as school size (and the impact of dropping the null values), to understand if these initial findings are statistically significant. Having more data on each district, drop out rate and population could allow us to provide a better insight and futher accurate analysis. Utilizing visuals such as scatter plots may also help us to quickly determine any misleading data or help us establish if the trends are more reliable. 
