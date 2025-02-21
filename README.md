# Prediction of Customers Likely to Drop Bank Services 

Neural Network model designed to predict customer churn, optimizing for accuracy and computational efficiency.

Summary:

Is it possible to predict -which customers are highly likely to leave the bank within 6 months? I will design a ANN to answer the question.

A bank services dataset will be used to analyze customer behaviours and tendencies.

![dataset](https://github.com/user-attachments/assets/b83682e4-b7cb-4d04-8b30-be1f2be0da53)

The following observations were extracted using essential statistical libraries against this bank's dataset: 

- The average Age of all Customers is 39 years.
- 75% of Customers have been with the bank for about 7 years with and average of 5 years.
- The average Customer balance is 76.5k.
- 70% of all Customers have Credit Cards.
- The average salary of Customers is 100k.
- 50% of Customers are from France and the remaining half are equally divided between Germany and Spain.
  
  ![p4_stats](https://github.com/user-attachments/assets/b3e7958b-317e-40c1-832c-b1c6554e8c99)

Recommendations:

- Right off the bat, bank offerings must include services in three languages: French, German and Spanish.
- There are twice as many French customers, therefore the marketing and customer support and customer retention budgets should reflect the same.
- Bots or AI assistants should provide culture and language sensitivity to reflect customer's distribution.
- Important: EU AI Act applies to all 3 countries and the bank must follow these regulations with strict compliance.

Additional Observations from the Exploratory Data Analysis (EDA):

- A fairly large number of Customers are keeping a 0 balance in their accounts.
- More precisely 3,617 out of 10,000 (36.2%) or a third of all customers. Recommendations:
- More research is required in this area. A budget for research should be added to understand contributing factors and corrective actions, RCCAs (Root Cause Corrective Actions).
- Incentives should be studied to provide value-add to these customers as a win-win for them and for the bank.
- A fairly large number of Customers are no longer active customers within the last 6 months.
- More precisely 2037 out of 7963 (26.6%) or a quarter of all customers leave. This is not acceptable.
- Incentives should be studied to provide value-add to these customers as a win-win for them and for the bank.

![Cust_Gens](https://github.com/user-attachments/assets/abb09a0f-2e43-4ca1-8244-0470f2a5646f)

![Conf_Matrix](https://github.com/user-attachments/assets/06731121-3e21-4ca8-8e74-e1863d9d09c8)


# A Recommendation and Business Justification to design, construct and train a Neural Network Model to predict customer departures:

- A predictive NN model should be designed to anticipate Customer trends and provide opportunities to interject before is too late. (This project. :-) )
- Daily runs in production should provide 'alerts' whenever patterns are detected or treshold metrics are crossed with production or unseen data.
- The predictive model should be fine-tuned regularly to incorporate additional data values accounting for the preventative-actions and measure both their exit-recurrence effectiveness to the business and the efficiency of the model predictions.
- Transparency of Customer's Privacy protections should be auditable and test-demonstrated frequently as this model is predictive and could cause incorrect, even catastrophic communications to Customers and Regulators when biased.
  
![my_nn](https://github.com/user-attachments/assets/b5609ff1-a37a-49d9-be52-48bfde21e6b2)

# We will design 5 NN models, train them and then fine-tune the best one.

![models_to_train](https://github.com/user-attachments/assets/b17887f2-024a-4dc2-b3a1-f268431d2e87)

Some examples from intermediate results: Only Model 0 anf Model 5 are shown here. The entire set of models 0--5 is in the python notebook in the repository.

Model 0 - Layers Summary:

![model_0](https://github.com/user-attachments/assets/f801ba1a-a5b5-4f21-9ea6-4628c7f192ad)

Loss comparison for Training vs Validation data:

![model_0_loss](https://github.com/user-attachments/assets/f68fff9c-d996-473e-90b6-0d561eccf996)

Model 5 - Layers Summary:

![model_5](https://github.com/user-attachments/assets/e318382b-9143-4188-bc85-0dbc5c50cb78)

Loss comparison for Training vs Validation data:

![model_5_loss](https://github.com/user-attachments/assets/026760ba-5596-47f2-9065-0b0d06466655)

Summary of all the models performance metrics:

![Model Optimizations](https://github.com/user-attachments/assets/878ae61a-b7a3-419f-aff0-44d5cbd4df4e)

![best_model_performance](https://github.com/user-attachments/assets/23b04736-847e-45dc-b1a9-35b9f93ded0a)

After fine-tuning and optimizing the best trained model, it can be further used to make more accurate predictions:

![recommendations_for_predictions](https://github.com/user-attachments/assets/07f97b69-5b32-46c3-9f61-205f85c8a924)

