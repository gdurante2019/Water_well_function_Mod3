<h1>Table of Contents<span class="tocSkip"></span></h1>
<div class="toc"><ul class="toc-item"><li><span><a href="#Executive-Summary" data-toc-modified-id="Executive-Summary-1"><span class="toc-item-num">1&nbsp;&nbsp;</span>Executive Summary</a></span></li><li><span><a href="#The-Project-and-Analysis" data-toc-modified-id="The-Project-and-Analysis-2"><span class="toc-item-num">2&nbsp;&nbsp;</span>The Project and Analysis</a></span><ul class="toc-item"><li><span><a href="#Problem-statement" data-toc-modified-id="Problem-statement-2.1"><span class="toc-item-num">2.1&nbsp;&nbsp;</span>Problem statement</a></span></li><li><span><a href="#Crowdsourcing-algorithms-to-predict-non-functional-wells" data-toc-modified-id="Crowdsourcing-algorithms-to-predict-non-functional-wells-2.2"><span class="toc-item-num">2.2&nbsp;&nbsp;</span>Crowdsourcing algorithms to predict non-functional wells</a></span></li><li><span><a href="#My-approach-to-the-problem" data-toc-modified-id="My-approach-to-the-problem-2.3"><span class="toc-item-num">2.3&nbsp;&nbsp;</span>My approach to the problem</a></span><ul class="toc-item"><li><span><a href="#Exploratory-data-analysis-(EDA)-and-custom-functions-for-visualization-and-modeling" data-toc-modified-id="Exploratory-data-analysis-(EDA)-and-custom-functions-for-visualization-and-modeling-2.3.1"><span class="toc-item-num">2.3.1&nbsp;&nbsp;</span>Exploratory data analysis (EDA) and custom functions for visualization and modeling</a></span><ul class="toc-item"><li><span><a href="#Regional-information" data-toc-modified-id="Regional-information-2.3.1.1"><span class="toc-item-num">2.3.1.1&nbsp;&nbsp;</span>Regional information</a></span></li><li><span><a href="#Water-abundance-(quantity)" data-toc-modified-id="Water-abundance-(quantity)-2.3.1.2"><span class="toc-item-num">2.3.1.2&nbsp;&nbsp;</span>Water abundance (quantity)</a></span></li><li><span><a href="#Extraction-type" data-toc-modified-id="Extraction-type-2.3.1.3"><span class="toc-item-num">2.3.1.3&nbsp;&nbsp;</span>Extraction type</a></span></li><li><span><a href="#Dealing-with-very-large-feature-sets" data-toc-modified-id="Dealing-with-very-large-feature-sets-2.3.1.4"><span class="toc-item-num">2.3.1.4&nbsp;&nbsp;</span>Dealing with very large feature sets</a></span></li></ul></li><li><span><a href="#Modeling" data-toc-modified-id="Modeling-2.3.2"><span class="toc-item-num">2.3.2&nbsp;&nbsp;</span>Modeling</a></span><ul class="toc-item"><li><span><a href="#Algorithms-used" data-toc-modified-id="Algorithms-used-2.3.2.1"><span class="toc-item-num">2.3.2.1&nbsp;&nbsp;</span>Algorithms used</a></span></li><li><span><a href="#Addressing-class-imbalances" data-toc-modified-id="Addressing-class-imbalances-2.3.2.2"><span class="toc-item-num">2.3.2.2&nbsp;&nbsp;</span>Addressing class imbalances</a></span></li><li><span><a href="#Customized-functions-for-displaying-model-results" data-toc-modified-id="Customized-functions-for-displaying-model-results-2.3.2.3"><span class="toc-item-num">2.3.2.3&nbsp;&nbsp;</span>Customized functions for displaying model results</a></span></li></ul></li></ul></li></ul></li><li><span><a href="#Discussion-and-Results" data-toc-modified-id="Discussion-and-Results-3"><span class="toc-item-num">3&nbsp;&nbsp;</span>Discussion and Results</a></span><ul class="toc-item"><li><span><a href="#Discussion" data-toc-modified-id="Discussion-3.1"><span class="toc-item-num">3.1&nbsp;&nbsp;</span>Discussion</a></span><ul class="toc-item"><li><span><a href="#What-does-'performance'-look-like?" data-toc-modified-id="What-does-'performance'-look-like?-3.1.1"><span class="toc-item-num">3.1.1&nbsp;&nbsp;</span>What does 'performance' look like?</a></span></li><li><span><a href="#Better-model-performance-means-fewer-false-negatives" data-toc-modified-id="Better-model-performance-means-fewer-false-negatives-3.1.2"><span class="toc-item-num">3.1.2&nbsp;&nbsp;</span>Better model performance means fewer false-negatives</a></span></li><li><span><a href="#The-trade-off:--Accuracy-score-vs.-better-prediction-of-failing-wells" data-toc-modified-id="The-trade-off:--Accuracy-score-vs.-better-prediction-of-failing-wells-3.1.3"><span class="toc-item-num">3.1.3&nbsp;&nbsp;</span>The trade-off:  Accuracy score vs. better prediction of failing wells</a></span></li></ul></li><li><span><a href="#Selecting-features-and-parameters-for-modeling" data-toc-modified-id="Selecting-features-and-parameters-for-modeling-3.2"><span class="toc-item-num">3.2&nbsp;&nbsp;</span>Selecting features and parameters for modeling</a></span></li><li><span><a href="#Feature-Importances" data-toc-modified-id="Feature-Importances-3.3"><span class="toc-item-num">3.3&nbsp;&nbsp;</span>Feature Importances</a></span></li><li><span><a href="#Results-Summaries:--Models" data-toc-modified-id="Results-Summaries:--Models-3.4"><span class="toc-item-num">3.4&nbsp;&nbsp;</span>Results Summaries:  Models</a></span><ul class="toc-item"><li><span><a href="#Decision-Trees" data-toc-modified-id="Decision-Trees-3.4.1"><span class="toc-item-num">3.4.1&nbsp;&nbsp;</span>Decision Trees</a></span></li><li><span><a href="#Bagged-Trees" data-toc-modified-id="Bagged-Trees-3.4.2"><span class="toc-item-num">3.4.2&nbsp;&nbsp;</span>Bagged Trees</a></span></li><li><span><a href="#Random-Forest" data-toc-modified-id="Random-Forest-3.4.3"><span class="toc-item-num">3.4.3&nbsp;&nbsp;</span>Random Forest</a></span></li><li><span><a href="#Gradient-Boost-and-AdaBoost" data-toc-modified-id="Gradient-Boost-and-AdaBoost-3.4.4"><span class="toc-item-num">3.4.4&nbsp;&nbsp;</span>Gradient Boost and AdaBoost</a></span></li><li><span><a href="#XGBoost" data-toc-modified-id="XGBoost-3.4.5"><span class="toc-item-num">3.4.5&nbsp;&nbsp;</span>XGBoost</a></span></li><li><span><a href="#Support-Vector-Machines-(SVM)" data-toc-modified-id="Support-Vector-Machines-(SVM)-3.4.6"><span class="toc-item-num">3.4.6&nbsp;&nbsp;</span>Support Vector Machines (SVM)</a></span></li></ul></li><li><span><a href="#The-verdict:--XGBoost-(with-SVM-as-runner-up)" data-toc-modified-id="The-verdict:--XGBoost-(with-SVM-as-runner-up)-3.5"><span class="toc-item-num">3.5&nbsp;&nbsp;</span>The verdict:  XGBoost (with SVM as runner-up)</a></span></li></ul></li><li><span><a href="#Conclusions-and-possible-future-work" data-toc-modified-id="Conclusions-and-possible-future-work-4"><span class="toc-item-num">4&nbsp;&nbsp;</span>Conclusions and possible future work</a></span><ul class="toc-item"><li><span><a href="#Conclusions" data-toc-modified-id="Conclusions-4.1"><span class="toc-item-num">4.1&nbsp;&nbsp;</span>Conclusions</a></span></li><li><span><a href="#Possible-Future-Work" data-toc-modified-id="Possible-Future-Work-4.2"><span class="toc-item-num">4.2&nbsp;&nbsp;</span>Possible Future Work</a></span></li></ul></li><li><span><a href="#Link-to-Blog-post" data-toc-modified-id="Link-to-Blog-post-5"><span class="toc-item-num">5&nbsp;&nbsp;</span>Link to Blog post</a></span></li></ul></div>

# Predicting Water Well Status in Tanzania using Machine Learning

## Executive Summary

___The problem:___  The government of Tanzania seeks to provide clean water to all of its citizens, but over 40% of the population still lacks access to clean water.  The government collaborated with Taarifa, a non-profit organization, to create a database of all of the water supply projects in the country. Data for each water supply project includes information about the project’s geographic location, local water abundance and quality, technical information (e.g., type of well), funder, installer, project administration, and more.

___Crowdsourcing machine learning to predict well function:___ DrivenData, a social enterprise that works with mission-driven organizations, is hosting a competition to predict water well status using machine learning algorithms. The dataset provided by DrivenData contains data for 59,400 water supply projects. There are 39 features in this dataset and three target classes (well status = ‘functional’, ‘non-functional’, or ‘functional; needs repair’).  Thus, this is a **multi-class classification problem.**

___My approach:___ For this project, I developed functions to customize data visualizations during the exploration phase and evaluated several different supervised machine learning models for predicting water well status. I also employed a few different approaches to address class imbalances, significantly improving performance around costly ‘false-negative’ errors (predicting wells to be ‘functional’, when in fact they were ‘non-functional’ or ‘functional needing repair’).  

For an overview of the functions I developed and deployed, check out my blog post at https://github.com/gdurante2019/gdurante2019.github.io/blob/master/_posts/2020-07-22-data_science_toolbox_function_to_create_top_n_values.markdown.

___Findings:___ In this project, I found that there is a significant trade-off between 1) better overall test accuracy scores when using the original imbalanced class data, and 2) better performance in minimizing false negative errors by addressing class imbalances.  In fact, the problem with false negatives resulting from the use of imbalanced class data is so great that, for a model to be useful, the class imbalance issue _must_ be addressed.  To do this, I employed either SMOTE resampling or the class_weight='balanced' parameter (where available).

## The Project and Analysis

### Problem statement

The government of Tanzania is working to provide clean water to all of its citizens, but over 40% of the population still lacks access to clean water.  Furthermore, a significant percentage of the wells that have been installed over the years are either in need of repair or replacement.  Because of variety of well types and the highly distributed nature of well projects, it is difficult for the government to be able to assess a particular well's status at any given time.

### Crowdsourcing algorithms to predict non-functional wells 

In an effort to better understand the functional status of wells around the country, Tanzania has collaborated with Taarifa, a non-profit organization, to create a database of all of the water supply projects in the country. Data for each water supply project includes information about the project’s geographic location, local water abundance and quality, technical information (e.g., type of well), funder, installer, project administration, and more.

DrivenData, a social enterprise that works with mission-driven organizations, is hosting a competition to predict water well status using machine learning algorithms. 

https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/

<img src='images/DrivenData_Tanz_comp_homepage.png' height=70% width=70%>


The dataset provided by DrivenData contains data for 59,400 water supply projects. There are 39 features in this dataset and three target classes (well status = ‘functional’, ‘functional; needs repair’, or ‘non-functional’).  Thus, this is a _**multi-class classification problem.**_

### My approach to the problem
_**Note:**_  I used this dataset to satisfy the project requirement for supervised learning/ensemble methods that had been covered to that point in my data science immersive program, which included decision trees, random forests, bagged trees, boosted trees, and support vector machines.  I chose to evaluate as many algorithms with hyperparameter tuning as possible to get a better sense of how the various models performed given different inputs and hyperparameter settings.
#### Exploratory data analysis (EDA) and custom functions for visualization and modeling
Because of the large number of individual feature values (39 features and anywhere from 2 to 2000 values per feature), I did a lot of EDA and wrote functions to customize data visualizations during the exploration phase.  This helped me to see variation across features and geographies, and helped me to understand the literal and figurative landscape of water projects throughout the country.  

Following are some examples of data visualizations that I developed to help me work with the data during the data exploration phase and the modeling phase.
##### Regional information
Below is a graph of well functional status by region.  Note that the y-axis represents the number of wells for each region.  This gives a nice summary view of how many wells there are by region and how these wells are performing.

<img src='images/status_by_region.png' height=70% width=70%>

It was also interesting to take a look at a few other factors that might be important for well performance.  A different way of considering geographic influences was to visualize water abundance by region:

<img src='images/water_qty_by_region.png' height=70% width=70%>

A quick visual comparison of the water abundance with well status in each region suggestions a possible correlation between better well performance and water abundance in the region as "enough".  Of course, there are many other factors to consider, but this comparison does suggest that some additional insights may be obtained by looking at well performance status by the water abundance characterization at the site where the well was installed.

##### Water abundance (quantity)

Speaking of water abundance ("quantity"), we can also view well status by the water abundance ("quantity") at the well site.  The largest number of wells are in areas with the quantity designation "enough", and their performance appears to be the best of the 5 water abundance categories.  Wells in areas categorized as "dry" appear to have the worst performance.  We might consider additional data visualization cross-referencing well status by extraction type and by water abundance as next steps, but it is informative to have a baseline sense of well status across different features.   

<img src='images/status_by_water_qty.png' height=50% width=50%>

##### Extraction type
An obvious parameter of well performance to consider is the type of water extraction mechanism used by the well.  A few examples of visualizations for this parameter are provided below. The first shows the mix of different well extraction types by functional status:  

<img src='images/status_vs_extr_type.png' height=50% width=50%>

Another view of the same information gives us a way to see extraction type on the x-axis, number of wells on the y-axis, and the functional status in the stacked column.  This instantly gives us a sense of both the number of wells _and_ functional status _by extraction type_: 

<img src='images/status_extr_type_class.png' height=60% width=60%>

While these two charts are great for viewing the extraction status and performance in terms of all installed wells, we can't really see the well status for small categories (e.g., rope pump, wind-powered).  This is where a percentage stacked column chart can be really useful:  

<img src='images/status_by_extr_type_pct.png' height=60% width=60%>

##### Dealing with very large feature sets

Some features, such as ```funder``` and ```installer```, contain over 2000 unique values each, but the vast majority of water projects were funded or installed by a small percentage of funders or installers.  I wanted to be able to separate out the biggest players across water projects and aggregate the hundreds of very small or one-off players into a single column.  Therefore, I developed functions that allowed me to aggregate smaller players into an "other" category based on a "smaller-than-n" value--e.g., if n=100, then the function would show the top 100 installers by number of wells, with the remaining installers (over 1900) aggregated into "other installers".  (This would also allow me to view how the wells of all of the remaining funders or installers performed, if I wished.) 

I used this function not only for visualization but also for modeling--vastly reducing the number of parameters in the model while still maintaining information about those wells funded or installed by the small players. 

One visualization example:  I selected the top 40 funders of water projects and plotted the number of wells they've funded in descending order, and used stacked columns to show what proportion of wells funded by each funder are functional, functional but needing repair, or non-functional (needing replacement).  

<img src='images/status_by_top40_funder.png' height=80% width=80%>

Because there is such a steep drop off in the number of wells represented by each funder beyond the first 10 or so, it is hard to see the functional status of all of the water wells by each funder.  Here again, it's useful to plot functional status as a percentage stacked column:  

<img src='images/status_by_funder_pct.png' height=80% width=80%>

#### Modeling

##### Algorithms used 
This classification project was amenable to several supervised machine learning algorithms.  I created decision-tree, random-forest, bagged-trees, AdaBoost, XGBoost, and SVM models using standard python libraries, and used GridSearchCV for hyperparameter tuning.  

##### Addressing class imbalances 
I explored a few different approaches to address class imbalances--e.g., ```class_weight='balanced'``` and SMOTE.  Doing this significantly improved model prediction of non-functional wells, reducing costly ‘false-negative’ errors.

##### Customized functions for displaying model results
I wanted to be able to summarized certain model results in a roll-up report.  To accomplish this, it was necessary to develop several functions to enable me to view these rolled-up results in an easy-to-read table.  This allowed me to identify the most important features resulting from each model run.  An example of such an output follows:


There are many ways to address class imbalances.  Given where I was in the data science program curriculum and the supervised learning approaches being examined for this project, I used either SMOTE resampling or the `class_weight='balanced'` parameter.  Doing so allowed me to greatly improve prediction of non-functional wells.  **I was able to reduce false negative errors from ~75% to around 25-30%, depending on the modeling approach.**  





## Discussion and Results

### Discussion
Before providing summary results of the different models, it's worth spending a little time describing what "performance" means in the context of this project, as well as the rationale for how I settled on certain features and performance parameters.  

####  What does 'performance' look like?
Of course, the "best-performing" model should predict _all_ wells correctly--'functional', 'non-functional', and 'functional--needs repairs'.  Developing a model that can accomplish this is challenging, however, because the percentages of these three types of wells--these three "classes"--are quite different ("imbalanced"):
* Approximately 53% of wells are functional
* About 36% of wells are non-functional (needing to be replaced)
* ~11% of wells are functional but in need of repair

Machine learning models run with imbalanced classes often do a poor job accurately predicting the less abundant classes (non-functional and functional--needing repairs).  This is because the largest classes provide more data points during the 'learning' process, which tends to drive predictions towards the most common class (and away from the less common classes).  

In this case, the most _common_ class is 'functional', but the most _important_ classes to identify are 'non-functional' and 'functional--needs repair'.  Thus, model results must be evaluated in the context of what models and parameters do the best job of accurately predicting non-functional wells and wells needing repairs, AND minimizing the number of failing wells incorrectly labeled as functional.

#### Better model performance means fewer false-negatives
For this project, the "best" model will both correctly predict failing wells _**and**_ minimize Type I errors (false-negatives, or labeling failing wells as functional).  Why?  Because it's more important for failing wells to be correctly identified as failing--so that they get prompt attention--than it is for functional wells to be identified as functional. 

#### The trade-off:  Accuracy score vs. better prediction of failing wells
Imbalanced target classes create a real challenge.  When imbalanced classes are not addressed, models tend to do poorly when predicting smaller classes (resulting in greater numbers of false negatives, for example); when imbalanced classes are addressed, overall accuracy seems to suffer.  There's a trade-off between higher accuracy scores and accurate prediction of smaller classes.  

The good news is that the data scientist and stakeholders decide what constitutes good performance.  In some situations, higher accuracy scores will indeed be the goal of modeling.  In other situations, some other measures will take precedence.  The key is to clearly define the most important outcomes and focus analysis on these objectives.

### Selecting features and parameters for modeling

After some earlier experimentation with various features in model development, I selected a subset of features per the following:
* Features that gave better predictive results
* Features that were not duplicative (for example, using only one of the geographic features within the dataset--```region```, ```lga```, or ```subvillage```, but not all three).  
* The subset of features that I used in every model discussed here was as follows:  
  * ```funder``` or ```installer```
  * ```lga``` or ```region```
  * ```management```
  * ```payment```
  * ```water_quality```
  * ```quantity_group```
  * ```source```
  * ```extraction_type_class```
  * ```status_group```
  * ```waterpoint_type```
  * ```permit```
  * ```public_meeting```

To reduce computational load and feature overlap, I generally selected either ```funder``` OR ```installer```, but not both.  For these features, I used the "top 'n'" function I developed to select the 'n' largest funders or installers and consolidate all of the smaller funders or installers (those not in the top 'n' largest) into an "other" category.

### Feature Importances 
* At a macro level, I found that the features that showed up most frequently in the aggregate feature importance list were the following (roughly in order of importance):
     * Quantity ('dry', 'enough', 'insufficient', 'seasonal', or 'unknown')
     * Region or lga (depending on which was used in the model)
     * Waterpoint type (standpipe, borehole, improved spring, cattle trough, other)
     * Installer or funder (depending on which was used in the model)
     * Extraction type (e.g., gravity, hand pump, motor, submersible)
     * Source (e.g., river, spring, shallow well, rainwater harvesting)
     * Payment type (e.g., pay by bucket, pay by month, never pay)
* At a more granular level, the top 30 or so dummy variables tended to include a mix of:
     * Water abundance
     * Waterpoint type
     * Geographic location (e.g., LGA)
     * Extraction type
     * Installer/funder
     * Payment type
* I recommend looking more closely at these values, since they are likely to contain those specific values that have more wells needing replacement or repair

### Results Summaries:  Models

#### Decision Trees
* Original **imbalanced** target dataset
  * Best results: 'funder', 'region', n=250
  * Well status correctly predicted for 11,369 wells (76.56% accuracy)
  * **Correctly predicted 'non-functional' or 'functional-needs repair' status for 4138 wells (60.08%)**
  * Fewest # of false-negatives of any imbalanced DT model:  2482 (36% of all failing wells)
* Balanced target dataset: ```class_weight='balanced'``` _(confusion matrices shown below)_
  * Best results: 'installer', 'LGA', n=250 
  * Well status correctly predicted for 8,923 wells (60.09% accuracy)
  * **Correctly predicted 'non-functional' or 'functional-needs repair' status for 4334 wells (62.93%)**
  * Fewest # of false-negatives of any class_weight='balanced' DT model:  1159 (16.83% of all failing wells)
* Balanced target dataset:  **SMOTE**
  * Best results: 'installer', 'LGA', n=125
  * Well status correctly predicted for 9,034 wells (60.84% accuracy)
  * **Correctly predicted 'non-functional' or 'functional-needs repair' status for 4146 wells (60.20%)**
  * Fewest # of false-negatives of any SMOTE DT model:  1435 (20.84% of all failing wells)
  
Running the decision tree model with balanced data using ```class_weight='balanced'``` gives the best results in terms of the highest number of malfunctioning wells correctly identified (**4334** out of 6887 wells).

<img src='images/CM-DT-bal-inst-lga-250-pct.png' height=45% width=45%>

<img src='images/CM-DT-bal-inst-lga-250.png' height=45% width=45%>

#### Bagged Trees
The performance of bagged trees models was lackluster compared with other modeling approaches.  Details of these models can be viewed in the relevant section of the technical notebook.

#### Random Forest
* Original **imbalanced** target dataset
  * Model run with: 'funder', 'LGA', n=125
  * Well status correctly predicted for 11,350 wells (76.43% accuracy)
  * **Correctly predicted 'non-functional' or 'functional-needs repair' status for 3856 wells (56.0%)**
  * Number of false-negatives:  2857 (41.5% of all failing wells)
* Balanced target dataset: ```class_weight='balanced'``` _(confusion matrices shown below)_
  * Model run with: 'funder', 'LGA', n=125
  * Well status correctly predicted for 10,967 wells (77.1% accuracy)
  * **Correctly predicted 'non-functional' or 'functional-needs repair' status for 4835 wells (70.2%)**
  * Number of false-negatives:  1432 (20.8% of all failing wells)
* Balanced target dataset:  **SMOTE**
  * Model run with: 'funder', 'LGA', n=125
  * Well status correctly predicted for 10,726 wells (72.23% accuracy)
  * **Correctly predicted 'non-functional' or 'functional-needs repair' status for 4614 wells (67.0%)**
  * Number of false-negatives:  1648 (23.93% of all failing wells)
  
Running the random forest model with balanced data using ```class_weight='balanced'``` gives the best results in terms of the highest number of malfunctioning wells correctly identified (**4835** out of 6887 wells).

<img src='images/CM-RF-bal-fund-lga-125-pct.png' height=50% width=50%>

<img src='images/CM-RF-bal-fund-lga-125.png' height=50% width=50%>

#### Gradient Boost and AdaBoost
Similar (but worse than) bagged trees models, the performance of models using either gradient boost or AdaBoost was lackluster compared with decision trees and random forest approaches. See the technical notebook section "Ensemble Methods:  Gradient Boosting and AdaBoost..." for more details.

#### XGBoost
* Original **imbalanced** target dataset
  * Model run with: 'funder', 'LGA', n=125
  * Well status correctly predicted for 11,726 wells (77.0% accuracy)
  * **Correctly predicted 'non-functional' or 'functional-needs repair' status for 4691 wells (68.11%)**
  * Number of false-negatives:  1904 (**27.65%** of all failing wells)
* Balanced target dataset:  **SMOTE** (confusion matrices shown below)
  * Model run with: 'funder', 'LGA', n=125
  * Well status correctly predicted for 11,114 wells (74.84% accuracy)
  * **Correctly predicted 'non-functional' or 'functional-needs repair' status for 4892 wells (71.03%)**
  * Number of false-negatives:  1474 (**21.4%** of all failing wells)
  
Running the XGBoost model with SMOTE rebalanced data with funder, LGA, and n=125 gives the best results in terms of the highest number of malfunctioning wells correctly identified (**4892** out of 6887 wells).

<img src='images/CM-XGB-SMOTE-fund-lga-125-pct.png' height=50% width=50%>

<img src='images/CM-XGB-SMOTE-fund-lga-125.png' height=45% width=45%>

#### Support Vector Machines (SVM)
* Balanced target dataset: ```class_weight='balanced'```
  * Best performing model with kernel=rbf, gamma=100.0, C=1.0, 'funder', 'LGA', n=125
  * Well status correctly predicted for 10,034 wells (67.57% accuracy)
  * **Correctly predicted 'non-functional' or 'functional-needs repair' status for 5193 wells (75.4%)**
  * Number of false-negatives:  920 (**15.97%** of all failing wells)
  
Running the SVM model with rebalanced data (class_weight=balanced), Gamma=100.0, C=1.0, funder, LGA, and n=125 gives the best results of SVM models--and indeed all models examined here--in terms of the highest number of malfunctioning wells correctly identified (**5193** out of 6887 wells).

<img src='images/CM-SVM-bal-fund-lga-125-pct.png' height=50% width=50%>

<img src='images/CM-SVM-bal-fund-lga-125.png' height=45% width=45%>

### The verdict:  XGBoost (with SVM as runner-up)
* XGBoost, while having slightly higher numbers of false negatives than SVM, did better overall than any other model in accurately predicting well status 
* Support Vector Machines (SVM) models gave the best results in terms of accurately predicting failing wells and minimizing false negatives (below 1000, significantly better than any other model examined here)
* However, SVM had almost twice as many false-positives (functional wells labeled as non-functional or needing repair) as did XGB; XGB had approximately 1730 false-positives, while SVM had close to 3000
* Of all of the models I developed, I think that XGBoost does the best job of overall well prediction accuracy while minimizing costly false-negatives, and significantly reducing false-positives (which, although not as problematic as false-negatives in this case, should nevertheless be minimized)

## Conclusions and possible future work

### Conclusions

This project datasets includes almost 40 features, and some features (e.g., installer, funder) have over 2000 possible values.  This created lots of challenges for me as a student:  I was learning how to implement models using a number of different algorithms, while also having to figure out ways to make the modeling process more manageable.  

From a technical perspective, I used extensive EDA and data visualization to get a better understanding of the data and gain insights into which parameters were likely to be most important.  Developing custom functions to reduce the number of variables (top 'n' values in a feature) and automate some elements of the modeling also helped.  While this effort took a lot of effort, I think it was time well-spent in terms of developing my skills and increasing my understanding of, and intuition around, modeling parameters and approaches that are likely to yield better results for a particular situation.

But I think that applying common sense when reviewing the model results is just as important as developing technical skills for more efficient data handling.  **Is the model actually doing a good job at predicting which wells are failing** (maximizing true positives and minimizing false negatives)?  Or is it just getting the highest accuracy but neglecting to minimize errors (such as predicting a non-functional well to be functional)?  

In this case, I was initially focused on the accuracy score (since this is what the DrivenData competition website outlines as an important metric), but as I started developing my models, I realized that the accuracy scores weren't telling me much about how well the models was doing at predicting failing wells.  I needed to dig deeper into the model results and started looking closely at the confusion matrices.  When I did this, I observed that models run without addressing class imbalances were doing a poor job at predicted failing wells.  I really internalized the fact that class imbalances can cause real problems with model predictions--and these errors can have real-life consequences.

I came to understand that there was a tradeof between high overall model accuracy and minimizing false negative errors.  By developing multiple iterations of models from different algorithms, I gained a more thorough understanding of these tradeofs and what kinds of adjustments would be most advantageous with similar types of data sets.

Having lots of skill at data visualization and manipulation is great, but these skills on their own will not automatically result in models that actually do a good job at what they are meant to do.  It is also necessary to think through the results and examine what's going on underneath the high-level scores and summary statistics.

### Possible Future Work
* Additional modeling with subsets of dummy variables: 
  * Most models have many of the same dummy variables at the top of their feature importance lists
  * May want to explore whether a smaller subset of dummy variables, such as the top 50, would improve model performance
* Improving data completeness--could additional information could be obtained for features with significant missing values or data entry inconsistencies?  For example:
  * ‘Other’ in the category ‘extraction_type’; almost 85% of wells in this category are non-functional
  * Year constructed--no date recorded for significant percentage of wells; do these wells have something in common, such as:
    * Clustered in certain locations where data was/is not collected?
    * Constructed before a certain date?
    * Constructed by certain installers or funded by certain funders?
    * Of a certain type, e.g., handpump?  
* Evaluating whether funder or installer country of origin influences well functionality
  * If the government of Tanzania or Taarifa had a complete and accurate list of the location for each funder/installer, the locations of the funders or installers could be another feature on which to model 
* Latitude / longitude—Looking at functional status of wells at various geographic locations to identify possible patterns due to geological differences
