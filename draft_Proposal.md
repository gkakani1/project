<div class="cell markdown" id="94bVfjUhHSIl">

# DATA 606: Capstone in Data Science

</div>

<div class="cell markdown" id="3xTRJYl8HuNt">

## Contents

## 1\) Draft Proposal

### 1.1 <a href='#1.1'>What is your issue of interest (provide sufficient background information)?</a>

### 1.2 <a href='#1.2'> Why is this issue important to you and/or to others?</a>

### 1.3 <a href='#1.3'>What questions do you have in mind and would like to answer?</a>

### 1.4 <a href='#1.4'>Where do you get the data to analyze and help answer your questions (creditability of source, quality of data, size of data, attributes of data. etc.)?</a>

### 1.5 <a href='#1.5'>What will be your unit of analysis (for example, patient, organization, or country)? Roughly how many units (observations) do you expect to analyze?</a>

### 1.6 <a href='#1.6'>What variables/measures do you plan to use in your analysis (variables should be tied to the questions in \#3)?</a>

### 1.7 <a href='#1.7'>What kinds of techniques/models do you plan to use (for example, clustering, NLP, ARIMA, etc.)?</a>

### 1.8 <a href='#1.8'>How you plan to develop/apply ML and how you evaluate/compare the performance of the models?</a>

### 1.9 <a href='#1.9'>What outcomes do you intend to achieve (better understanding of problems, tools to help solve problems, predictive analytics with practicle applications, etc)?</a>

</div>

<div class="cell markdown" id="_43N8-uiJWM7">

## 1.1) What is your issue of interest (provide sufficient background information)? <a id ="1.1"></a>

</div>

<div class="cell markdown">

### Aim: - Suggesting best trading option for a perishable food crop for a state among the states across India.

Perishable foods such as fruits and vegetables have a limited self-life
after harvest or production. Most of these crops must be traded with in
1-2 weeks of harvesting. Through this capstone project I am planning to
design an algorithm which can suggest a particular state in India about
what are the best set of states to trade a particular crop. If a
particular crop is expected to get exported the algorithm should suggest
the states to trade with for high profit margins or else in case of
importing a perishable food crop the suggestions should be made to
minimize the import price of the crop.

### Other Issues that can be addressed: -

\(\rightarrow\) Predicting most profitable crop for that season

\(\rightarrow\) Helping traders to make high profit margins

</div>

<div class="cell markdown" id="-h3LQaF9Js1B">

## 1.2) Why is this issue important to you and/or to others? <a id ="1.2"></a>

</div>

<div class="cell markdown">

India is an agricultural country and one third population depends on the
agricultural sector directly or indirectly. Agriculture remains as the
main stray of almost all Indian states economy. The primary income for
large sector of people in each state in India is agriculture and most of
the state produces same set of different variety of crops. Indian
agriculture mostly depends on rainfall and other climatic conditions.
India is a peninsula as it is surrounded by 3 different water bodies on
three sides each state will be experiencing different climatic
conditions which in turn effects the crop production. I am choosing
perishable crops (Mostly fruits and vegetables) because unlike cash
crops perishable crops should be transported and use within 1-2 weeks of
harvesting. As seasonal weather forecast for is more reliable, I want to
build a model such that both government and farmers can plan efficiently
to reach their desirable margins. Using this recommendation system
government can plan imports and exports across the country to increase
farm profitability. Trade plays a crucial role in providing livelihoods
for farmers and people employed along the food supply chain. A
well-planned trade model in case of exports will bring good revenue for
sate government and farm price for their crop. The government can
estimate the import prices of perishable crops and can try to minimize
the price as much as they can.

</div>

<div class="cell markdown" id="1JAmlhq5JtRN">

## 1.3) What questions do you have in mind and would like to answer? <a id ="1.3"></a>

</div>

<div class="cell markdown">

\(\rightarrow\) What are the best set of sates to export a perishable
food crop for higher food margins?

\(\rightarrow\) What are the best set of states to import a perishable
crop at lower price?

\(\rightarrow\) What is the best perishable food crops to plant in a
particular season at a particular state?

\(\rightarrow\) For a particular vegetable or food crop in a particular
season what can be the highest expected farm price?

\(\rightarrow\) For a particular crop at a particular season is it
possible to make desirable profit?

</div>

<div class="cell markdown" id="F37v8m08Jtdx">

<a id ="1.4"></a>

## 1.4) Where do you get the data to analyze and help answer your questions (creditability of source, quality of data, size of data, attributes of data. etc.)?

</div>

<div class="cell markdown">

Below are the datasets which I require for this project and their
details.

### 1)Monthly farm prices of different cops at different states across the country.

\(\rightarrow\) Note: - In my project I am taking top 10 most produced
perishable crop datasets from Jan 2020 till Dec 2021 into consideration
and work on them.

\(\rightarrow\) Source: - National Horticulture Board of India

\(\rightarrow\) Link: -
<http://nhb.gov.in/OnlineClient/MonthlyPriceAndArrivalReport.aspx?enc=3ZOO8K5CzcdC/Yq6HcdIxJ4o5jmAcGG5QGUXX3BlAP4=>

\(\rightarrow\) Link to Dataset in my Google Drive(Anyone from UMBC
group can access it): -
<https://drive.google.com/drive/folders/1OxtPZU1gt_ehgOiGhl_hpdmPWlvjO2ZW?usp=sharing>

\(\rightarrow\) Attributes of the datasets: - Each individual dataset
consists of 6 attributes, namely

  - Centre Name: - Name of the state

  - Year: - Year in which data is collected

  - Month: - Month in which data is collected

  - W.sale avg.price: - Sale Price in rupees per quintal(100kg)

  - Retail Avg.price: - Retail Price in rupees per quintal

  - Total Arrival: - Arrival in metric tons(1000)

### 2)Monthly weather report of each and every sate in India from 2010 to 2020.

\(\rightarrow\) Source: - NASA’s Data Access Viewer: - Its Provides
solar and meteorological data sets from NASA research for support of
renewable energy, building energy efficiency and agricultural needs.

\(\rightarrow\) Link: -
<https://power.larc.nasa.gov/data-access-viewer/>

\(\rightarrow\) Link to Dataset in my Google Drive(Anyone from UMBC
group can access it):-
<https://drive.google.com/drive/folders/15zXCuLByVlfpdg5eg_yfT2qBmqdDHeif?usp=sharing>

\(\rightarrow\) Attributes of the Datasets: -

  - All Sky Surface PAR Total:- The total Photosynthetically Active
    Radiation (PAR) incident on a horizontal plane at the surface of the
    earth under all sky conditions.

  - Dew/Frost Point at 2 Meters:- The dew/frost point temperature at 2
    meters above the surface of the earth.

  - Temperature at 2 Meters Maximum:- The maximum hourly air (dry bulb)
    temperature at 2 meters above the surface of the earth in the period
    of interest.

  - Temperature at 2 Meters Minimum:- The minimum hourly air (dry bulb)
    temperature at 2 meters above the surface of the earth in the period
    of interest.

  - Specific Humidity at 2 Meters:- The ratio of the mass of water vapor
    to the total mass of air at 2 meters (kg water/kg total air).

  - Precipitable Water:- The total atmospheric water vapor contained in
    a vertical column of the atmosphere.

  - Wind Speed at 2 Meters Maximum: - The maximum hourly wind speed at 2
    meters above the surface of the earth.

  - Wind Speed at 2 Meters Minimum: - The minimum hourly wind speed at 2
    meters above the surface of the earth.

  - Surface Soil Wetness:- The percent of soil moisture a value of 0
    indicates a completely water-free soil and a value of 1 indicates a
    completely saturated soil; where surface is the layer from the
    surface 0 cm to 5 cm below grade.

  - Root Zone Soil Wetness:- The percent of root zone soil wetness a
    value of 0 indicates a completely water-free soil and a value of 1
    indicates a completely saturated soil; where root zone is the layer
    from the surface 0 cm to 100 cm below grade.

  - Profile Soil Moisture: - The percent of profile soil moisture a
    value of 0 indicates a completely water-free soil and a value of 1
    indicates a completely saturated soil; where profile is the layer
    from the surface down to the bedrock.

\(\rightarrow\) Total data size: 50MB

</div>

<div class="cell markdown" id="Rh0NfSRqJto9">

## 1.5) What will be your unit of analysis (for example, patient, organization, or country)? Roughly how many units (observations) do you expect to analyze?<a id ="1.5"></a>

</div>

<div class="cell markdown">

\(\rightarrow\) My unit of analysis is the farm price data of a
perishable food crop associated with individual sates (29) in India .

</div>

<div class="cell markdown" id="hfptodh-Jtzd">

## 1.6) What variables/measures do you plan to use in your analysis (variables should be tied to the questions in 3)?<a id ="1.6"></a>

</div>

<div class="cell markdown">

\(\rightarrow\) I am thinking to use historical weather data attributes
in predicting the farm price of a perishable food crop. I am planning to
select the features after doing exploratory data analysis. I am going to
consider the factors such as number of null values for a given feature,
outliers and anomalies persent in the features along with the help of
heatmap in feature selection.

</div>

<div class="cell markdown" id="-u8T3ws9Jt8p">

## 1.7) What kinds of techniques/models do you plan to use (for example, clustering, NLP, ARIMA, etc.)? <a id ="1.7"></a>

</div>

<div class="cell markdown">

\(\rightarrow\) I will be using supervised learning techniques in my
algorithm

\(\rightarrow\) As of now I think of two different techniques to design
the model

  - Using Multi-Class Classification Algorithms: I will try to train my
    model using multi-class classification machine learning algorithms
    such as k-Nearest Neighbor’s, Decision Trees, Naive Bayes etc...

  - Using regression methods: Training my model using regression
    algorithms such as Neural Network Regression or LASSO regression
    etc...

</div>

<div class="cell markdown" id="Lsoz28ucJuF9">

## 1.8) How do you plan to develop/apply ML and how you evaluate/compare the performance of the models? <a id ="1.8"></a>

</div>

<div class="cell markdown">

\(\rightarrow\) For Multi-Class classification: - Under this Multi-Class
classification I plan to divide the farm price of each crop into 3 or 4
different slabs such as high profit margin, low profit margin or loss
and predict under which slab a particular crop can fall given all the
features. In case of multi-Class classification I will be using
confusion matrix to compare the performance of models using Precision
and Recall values. I can also use the F1 score to compare the
performance among trained models.

\(\rightarrow\) Using regression methods: - My second thought is to use
regression algorithms to train my model and predict the farm price of a
perishable food crop. To choose the best regression model I can use
metrics such as Correlation Coefficient or Mean Square Error and Mean
Absolute Error.

</div>

<div class="cell markdown" id="kGjl-oc5JuRi">

## 1.9) What outcomes do you intend to achieve (better understanding of problems, tools to help solve problems, predictive analytics with practicle applications, etc)? <a id ="1.9"></a>

</div>

<div class="cell markdown" id="jmo5Z4P1Hktq">

\(\rightarrow\) After traing my model I aim to suggest the best states
to trade with for a pirticular crop in a specific state. I am planning
to use different chart and plots using visualization tools such as
Matplotlib, Seaborn to make it much effective.

</div>
