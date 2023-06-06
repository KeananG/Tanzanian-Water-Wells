# Tanzanian-Water-Wells
![Tanzania](https://www.wvi.org/sites/default/files/2022-06/Water%20for%20Change%20-%20Tanzania.png)
# <center> Phase 3 Project: Tanzanian Water Wells <center>
   <center>  By: Keanan Ginell
# Business Overview
 Access to water is a basic human right, yet it remains a persistent challenge in economically disadvantaged nations. This is an issue faced by citizens of these nations on a daily basis. Recognizing the significance of ensuring water accessibility for the people of Tanzania, this model aims to determine the functionality of wells and identify those that require repair. The key parties involved in addressing this problem include the Tanzanian government, the citizens of Tanzania, and the individuals engaged in the repair of water wells. 


# Method
In order to achieve this, I initially constructed a dummy model utilizing this as my basline model. Subsequently, I assessed various other models, including a decision tree, logistic regression, and random forest. Upon determining that the random forest model exhibited the highest performance, I optimized the models parameters using a pipeline and grid searches. As a result, I developed a final model that achieved an accuracy of 81%, which is significantly superior to the baseline model's accuracy of 54%.

# Results

![Feature Importance](feature_importance.png)

      Among the various features considered, the most crucial one is GPS Height, and there are several potential reasons for its significance. Firstly, there may exist a correlation between the altitude of a well and other inherent attributes that are typically associated with different altitudes. Secondly, the type of well pump utilized may vary at different altitudes, subsequently affecting its functional capacity. The remaining important features, such as the well's age, water availability, and TSH, were expected to contribute more significantly to the overall analysis.
      
![scores](scores.png)
# Wells gps height
![well_locations](well_locations.png)

# Wells Functionality
![well_locations3](well_locations3.png)





   
 # Conclusion

Comparing the accuracy and recall scores from the baseline model to the final model, 

Baseline:
- Accuracy - 57%
- Recall - 57%

Final Model:
- Accuracy - 81%
- Recall - 81%

The final model used in this approach is a random forest with optimized parameters. This model serves the purpose of predicting the status of a well, whether it is functional, non-functional, or functional but in need of repair. Given that access to safe and clean water is considered a fundamental human right, these wells play a vital role in ensuring access to clean water. By utilizing my model, the Tanzanian government can effectively assess whether a well requires repair, aiding in their decision-making process. 
      As I look ahead to the next steps, I am planning to revise the process of developing a predictive model. Initially, I will create a binary classification model with the aim of improving the accuracy of predicting whether a well is functional or not. This binary model will be generated twice, with wells needing repair categorized differently in each model. Once the optimal split for the three classes is determined, a second model will be constructed to predict within the class that contains functional wells but needs repair. This second model will identify which wells specifically need repair. The objective is to enhance the accuracy of predicting the three classes by utilizing two binary classification models as opposed to the current three class model.

ion
