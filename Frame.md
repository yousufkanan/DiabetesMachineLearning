# Frame the Problem

- Define the objective in business terms?
    - The objective is to predict weather a 
    patient admitted to the hospital for diabetes will be readmitted within 30 days.
- How will your solution be used?
    - The solution will be used to help the hospital identify patients who are at risk of being readmitted within 30 days. It will allow 
    us to both provide additional care to those patients and to allocate resources more effectively. These prediciotns will also allow us to measure the effectivness of individual
    care providers. 
- What are the current solutions/workarounds (if any)?
    - Currently, hospitals use 
- How should you frame this problem (supervised/unsupervised, online/offline, etc.)?
    - This is a supervised learning problem as we have labeled data. Ideally we would like to test the model in an online setting
     but we will start with an offline setting.
- How should performance be measured?
    - Performance will be measured by the f1-score of the model. This is because both precision and recall are very important in this case. There 
    might be slight preference for recall as we would like to catch as many of the patients who are at risk of being readmitted as possible.
- What would be the minimum performance needed to reach the business objective?
    - The minimum performance needed to reach the buisness objective would be a f1-score of 0.7. This is because we want a solid model, 
    but we understnad that there will be some false positives and false negatives.
- What are comparable problems? Can you reuse experience or tools?
    - This is a classification problem like many others. We can use a model shortlist from HW4 (include ADA Boost). We can also do 
      some feature augmentation with other data like we did in previous projects.
- Is human expertise available?
    - No, we do not have human expertise available.
- How would you solve the problem manually?
    - We would look at the data and try to identify patterns that are associated with patients who are readmitted within 30 days. 
    We would then use these patterns to predict which patients are at risk of being readmitted.
    We could also rely on the intuition of doctors and nurses to help us identify these patterns.
- List the assumptions you (or others) have made so far.
    - We have assumed that the data is clean and that the labels are accurate.
    - We have assumed that the data is representative of the population of patients that we are interested in.
    - We have assumed that the features in the data are relevant to the problem.
    - We have not assumed that the features are independent of each other.
    - We have not assumed that the data is randomly sorted already 