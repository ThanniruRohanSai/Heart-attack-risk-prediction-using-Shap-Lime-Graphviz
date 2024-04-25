# Heart-attack-risk-prediction-using-Shap-Lime-Graphviz
This project investigates the use of SHAP (SHapley Additive exPlanations) and LIME (Local Interpretable Model-Agnostic Explanations) for interpreting machine learning models in predicting heart attack risk.

Data and Models:

The project utilizes a dataset containing information on various factors potentially affecting heart attack risk.
Two machine learning models are employed for risk prediction:
Decision Tree Classifier
Random Forest Classifier
SHAP is used to explain the global feature importances for the decision tree model, while LIME is used to provide local explanations for individual predictions from the random forest model.
Initial Observations from SHAP Values (10 Instances):

thal: High average positive SHAP value suggests a strong association with increased heart attack risk.
age: Positive SHAP values indicate that age is also a significant contributor to higher risk, aligning with medical knowledge.
cp (chest pain type): Positive SHAP values suggest chest pain type has a positive influence on risk prediction.
Further Analysis of Features with Negative SHAP Values:

exang (exercise-induced angina): Negative SHAP values might indicate a negative association with risk. Individuals with exercise-induced angina might be more likely to seek medical attention and potentially have underlying conditions managed.
fbs (fasting blood sugar): Negative SHAP values might suggest a link to lower risk. However, it's crucial to investigate this further as low blood sugar can also be dangerous.
Decision Tree Visualization with Graphviz:

A decision tree visualization is created using Graphviz to provide a visual representation of the decision-making process within the decision tree model. This can help in understanding how different features interact to influence the final risk prediction.
Disclaimer:

The findings from this analysis are based on a limited sample of ten instances. A more comprehensive analysis with a larger dataset is recommended for robust conclusions.
While negative SHAP values for exang and fbs suggest potential associations, further medical expertise is necessary to interpret these relationships in the context of heart attack risk assessment.
Future Work:

Analyze a larger dataset to validate the initial observations and gain more robust insights.
Explore the use of SHAP with the Random Forest model for a more comprehensive feature importance analysis.
Investigate feature interactions to understand how combinations of features influence risk prediction.
Incorporate additional machine learning models and compare their performance and interpretability.
By leveraging SHAP and LIME, this project demonstrates the potential of explainable AI techniques in understanding complex models used for heart attack risk prediction. These interpretable insights can be valuable for medical professionals and data scientists alike, aiding in better decision-making and risk assessment for heart patients.
