# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required packages.
2.Read the data set.
3.Apply label encoder to the non-numerical column inoreder to convert into numerical values.
4.Determine training and test data set.
5.Apply decision tree Classifier and get the values of accuracy and data prediction.
## Program:

/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: SHAIK MUFEEZUR RAHAMAN
RegisterNumber: 212221043007
import pandas as pd
data=pd.read_csv("Employee.csv")
data.head()

data.info()

data.isnull().sum()

data["left"].value_counts()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()

x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()

y=data["left"]

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)

from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)

y_pred=dt.predict(x_test)

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy

dt.predict([[0.5,0.8,9,260,6,0,1,2]])

*/

## Output:

![275272196-817f7be7-9690-4757-9057-9219f8692920](https://github.com/githubmufeez45/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/134826568/780a0332-2a55-403a-bf0d-c393c0119b9e)

![275272212-db3ce613-5b04-44f5-a4e8-a03c0fcbd00d](https://github.com/githubmufeez45/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/134826568/9601f3db-8b52-4100-bf1b-3ff1a408288e)

![275272229-60e3223c-61ef-4657-97ee-82a45b3fc9a8](https://github.com/githubmufeez45/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/134826568/797e94cc-0f5a-4685-9b02-ac078cb11c15)

![275272238-56123f56-5e2e-4e37-af46-14f4d69d88c8](https://github.com/githubmufeez45/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/134826568/618df130-c3a8-4349-9feb-0e8fdcd253c0)

![275272279-d1d3278b-fd7c-4c91-85b5-ac905d80da42](https://github.com/githubmufeez45/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/134826568/64a50c2f-e3b9-4d75-bef2-c6ebea838700)

![275272300-34b32e3d-bc6b-4eeb-884d-138a60e320c5](https://github.com/githubmufeez45/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/134826568/b42b0f1e-e601-40d9-9b7b-25f47d2a1674)

![275272309-a6b650e5-e936-4d1b-951d-567416efc9e8](https://github.com/githubmufeez45/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/134826568/6225cb4e-19e8-430e-b373-2204e65b6f2f)

![275272320-954c446d-8baa-4095-afd0-2624bc76a814](https://github.com/githubmufeez45/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/134826568/d892f590-7b61-46ed-9d86-6d72f53cf483)



## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
