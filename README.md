Data Visualizations
==============================

Story telling and visualization to describe the 120 years of Olympics data, dating from 1896 to 2016.

For the analysis, **"Jupyter notebooks"** and **"Tableau**" are used.
  
Data sets are collected from previous project "Jimmy Wrangler - Data Exploration" 
[here](https://github.com/mugdhabajjuri/Datascience1)

# Story telling in Jupyter Notebook


## Distribution of the age of gold medalists



![png](reports/first.png)


### There are people who have won gold medals with Age greater than 50 😲😲😲

#### let's see how many people won gold medals after turning 50 🏅


```python
goldMedals['ID'][goldMedals['Age'] > 50].count()
```




    65



### 🕕🕔 people!!!  That's great

### Let's dive deep into age of the olympic participants


![png](reports/second.png)


### Two things to observe here :
#### - There are participants, whose age is over 80 👏
#### - In 1904 female age distribution is strongly different from the other Olympics



### ART COMPETITIONS --- I did not know that the Olympics include Art Competitions!!

### Female age distribution in 1904











### Height vs Weight of Olympic Medalists




![png](reports/third.png)


From above graph it can be seen that the more the weight, the more the height i.e., linear relation

### Let's athelets whose weight is more than 160 kilograms


```python
notNullMedals.loc[notNullMedals['Weight'] > 160]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>ID</th>
      <th>Name</th>
      <th>Sex</th>
      <th>Age</th>
      <th>Height</th>
      <th>Weight</th>
      <th>Team</th>
      <th>NOC</th>
      <th>Games</th>
      <th>Year</th>
      <th>Season</th>
      <th>City</th>
      <th>Sport</th>
      <th>Event</th>
      <th>Medal</th>
      <th>region</th>
      <th>notes</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>39181</th>
      <td>20144</td>
      <td>Andrey Ivanovich Chemerkin</td>
      <td>M</td>
      <td>24.0</td>
      <td>183.0</td>
      <td>170.0</td>
      <td>Russia</td>
      <td>RUS</td>
      <td>1996 Summer</td>
      <td>1996</td>
      <td>Summer</td>
      <td>Atlanta</td>
      <td>Weightlifting</td>
      <td>Weightlifting Men's Super-Heavyweight</td>
      <td>Gold</td>
      <td>Russia</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>268659</th>
      <td>134407</td>
      <td>Leonid Ivanovych Zhabotynskiy</td>
      <td>M</td>
      <td>26.0</td>
      <td>189.0</td>
      <td>163.0</td>
      <td>Soviet Union</td>
      <td>URS</td>
      <td>1964 Summer</td>
      <td>1964</td>
      <td>Summer</td>
      <td>Tokyo</td>
      <td>Weightlifting</td>
      <td>Weightlifting Men's Heavyweight</td>
      <td>Gold</td>
      <td>Russia</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>268660</th>
      <td>134407</td>
      <td>Leonid Ivanovych Zhabotynskiy</td>
      <td>M</td>
      <td>30.0</td>
      <td>189.0</td>
      <td>163.0</td>
      <td>Soviet Union</td>
      <td>URS</td>
      <td>1968 Summer</td>
      <td>1968</td>
      <td>Summer</td>
      <td>Mexico City</td>
      <td>Weightlifting</td>
      <td>Weightlifting Men's Heavyweight</td>
      <td>Gold</td>
      <td>Russia</td>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
</div>



### Ah! Weighlifters!! ---- that makes sense 🏋️‍♂️


