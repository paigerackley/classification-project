# <center><a name="top"></a>Classification Project: Telco Churn 
![](images/telco.jpeg)

by: Paige Rackley </center>

<p>
  <a href="https://github.com/paigerackley" target="_blank">
    <img alt="Paige" src="https://img.shields.io/github/followers/paigerackley?label=Follow_Paige&style=social" />
  </a>

 * * *  
[[Project Description](#project_description)]
[[Project Planning](#planning)]
[[Key Findings](#findings)]
[[Data Dictionary](#dictionary)]
[[Data Acquire and Prep](#wrangle)]
[[Data Exploration](#explore)]
[[Statistical Analysis](#stats)]
[[Modeling](#model)]
[[Conclusion](#conclusion)]
___



## <a name="project_description"></a>Project Description:
  > - Document code, process (data acquistion, preparation, exploratory data analysis and statistical testing, modeling, and model evaluation), findings, and key takeaways in a Jupyter Notebook Final Report.
  > - Create modules (acquire.py, prepare.py) that make my process repeateable and easy to follow.
  > - Explore data that will help to understand the drivers of customers churning. Answer questions that arise using charts and statistical tests.
  > - Construct a model to predict customer churn using classification techniques, and make predictions for a group of customers.
  > - Refine work and processes into a Final Report that shows what work was done, my goals, what I found and my conclusions.
[[Back to top](#top)]

***
## <a name="planning"></a>Project Planning:
  
  
 ### Business Goals: 
 > - Find drivers for customer churn at Telco. Why are customers churning?
 > - Construct a ML classification model that accurately predicts customer churn.
 > - Deliver a report that a non-data scientist can read through and understand.

 ### Audience:
> - My target audience is for fellow Codeup Students and staff. 
        
### Initial Hypothesis: Churn is most directly associated with 4 factors: Senior citizens, electronic checks, fiber optic internet, and tech support

## Hypothesis:
  
# Question1: Is churn associated with senior citizens?
  - H0: Rate of churn is not dependent on being a senior citizen.
  - H1: Rate of churn is dependent on being a senior citizen.
  
# Question2: Is churn associated with fiber optic internet?
  - H0: Churn is not dependent on having fiber optic internet.
  - H1: Churn is dependent on having fiber optic internet.

# Question3: Is churn associated with customers who use electronic checks for payments?
  - H0: Churn is not dependent on electronic check payment type.
  - H1: Churn is dependent on electronic check payment type.
 
# Question4: Is churn associated with those who don't receive tech support?
  - H0: Churn is not dependent on if a customer receives tech support.
  - H1: Churn is dependent on if a customer receives tech support.
  
### Deliverables:
> - A final report notebook
> - A final report notebook presentation
> - All necessary modules to make my project reproducible


### Nice to haves (With more time):
> - On your best model, a chart visualizing how it performed on test would be valuable.


[[Back to top](#top)]

***

## <a name="findings"></a>Key Findings:
[[Back to top](#top)]




***

## <a name="dictionary"></a>Data Dictionary  
[[Back to top](#top)]

### Data Used
  
Target|Datatype|Definition|
|:-------|:--------|:----------|
| churn | 7043 non-null: object | customer churn Yes or No |

|Feature|Datatype|Definition|
|:-------|:--------|:----------|
| internet_service_type_id       | 7043 non-null: int64 |    id refering to type of internet service used |
| payment_type_id        | 7043 non-null: int64 |    id refering to type of payment used |
| contract_type_id       | 7043 non-null: int64 |    id refering to type of contract used |
| customer_id        | 7043 non-null: object |    individual customer id string |
| gender       | 7043 non-null: object |    customer male or female |
| senior_citizen        | 7043 non-null: int64 |    is customer senior |
| partner       | 7043 non-null: object |    does customer have a partner |
| dependents        | 7043 non-null: object |    does customer have dependents |
| tenure       | 7043 non-null: int64 |    length customer with company in months |
| phone_service        | 7043 non-null: object |    uses phone service Yes or No |
| multiple_lines       | 7043 non-null: object |    Yes, No, or No phone service |
| online_security        | 7043 non-null: object |    Yes, No, No internet service |
| online_backup       | 7043 non-null: object |    Yes, No, No internet service |
| device_protection        | 7043 non-null: object |    Yes, No, No internet service |
| tech_support       | 7043 non-null: object |    Yes, No, No internet service |
| streaming_tv        | 7043 non-null: object |    Yes, No, No internet service |
| streaming_movies       | 7043 non-null: object |    Yes, No, No internet service |
| paperless_billing        | 7043 non-null: object |    uses paperless billing Yes or No |
| monthly_charges       | 7043 non-null: float64 |    monthly bill amount in USD |
| total_charges        | 7043 non-null: object |    lifetime total charged to customer in USD  |
| contract_type       | 7043 non-null: object |    One Year, Two Year, Month-to-month |
| payment_type        | 7043 non-null: object |    Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic)|
| internet_service_type       | 7043 non-null: object |    Fiber optic, DSL, None |
***

## <a name="wrangle"></a>Data Acquisition and Preparation
[[Back to top](#top)]

![]()



  
## <a name="explore"></a>Data Exploration:
[[Back to top](#top)]
- Python files used for exploration:



### Takeaways from exploration:


***

## <a name="stats"></a>Statistical Analysis
[[Back to top](#top)]


***

## <a name="model"></a>Modeling:
[[Back to top](#top)]



## <a name="conclusion"></a>Conclusion:
[[Back to top](#top)]
  
  
  **How to Reproduce**
- [x] Read this README.md
- [ ] Download the aquire.py and prepare.py into your working directory
- [ ] Have fun doing your own exploring, modeling, and more! 

