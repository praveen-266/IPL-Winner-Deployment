
# IPL-Winner-Prediction-Deployment         

# Proble Statement 
Indian Premier League (IPL) ia a famous twenty-20 League conducted by the Board of Control for Cricket in india (BCCI). It was started in 2008 and successfully completed fourteen seasons till 2021. IPL is a popular sport where it has large set of audience throughout the country. Every cricket fan would be eager to know and predict the IPL match result. A solution using Machine Learning is provided for the innings score considering the past data of match by match and ball by ball. Match winner prediction is taken as classification problem. Algorithms like Logistic Regression and RandomForest are used for classification of match winner.      

# Approach 

## 1.Exploaratory Data Visualization          
Statistical data analysis and Data Visualization performed on data to find if any outlier or missing data are present          

## 2. Data Preprocessing       
* we got Nan/missing values more than 90% in features like "Fielder_involved" , "Kind", "player_out", "extra_type". So , I removed them      
* Removed Old names and updated with new names of Teams      
* we need to focus on second innings only to predict winner of the match

## 3. Feature Engineering       
created some features based on firtst innings for second innings:
      * current_score
      * runs_left
      * wicket_left 
      * balls_left        
      * current_run_rate           
      * required_run_rate         
## 4. final dataframe features to predict:       
"BattingTeam", "BowlingTeam", "City" , "Target" , "runs_left", "balls_left", "wicket_lefts", "current_lefts", "required_run_rate" , "result"         

## 5. Model Training          
i tried several base models such as LogisticRegression, RandomForest Classifier, DecisionTreeClassifier using hyperparameter with GrisSearchCV validation. among these models **RandomForestClassifier** gives the best macro f1 score           

→ If you are searching for code, algorithms used . you won't find it here. Click the link mentioned below for the same:             
https://github.com/praveen-266/Machine-Learning-Projects/tree/main/IPL%20Winner%20Prediction

Do ⭐ the repository, if it helped you in anyway
