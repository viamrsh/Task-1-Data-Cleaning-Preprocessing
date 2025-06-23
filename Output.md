# output 
Drive already mounted at /content/drive; to attempt to forcibly remount, call drive.mount("/content/drive", force_remount=True).
<class 'pandas.core.frame.DataFrame'>

RangeIndex: 891 entries, 0 to 890

Data columns (total 12 columns):

     Column       Non-Null Count  Dtype
     0   PassengerId  891 non-null    int64  
    1   Survived     891 non-null    int64  
    2   Pclass       891 non-null    int64  
    3   Name         891 non-null    object 
    4   Sex          891 non-null    object 
    5   Age          714 non-null    float64
    6   SibSp        891 non-null    int64 
    7   Parch        891 non-null    int64  
    8   Ticket       891 non-null    object  
    9   Fare         891 non-null    float64
    10  Cabin        204 non-null    object 
    11  Embarked     889 non-null    object 
 
dtypes: float64(2), int64(5), object(5)

memory usage: 83.7+ KB

Initial Info:
 None
# Missing values:

    PassengerId      0
    Survived         0
    Pclass           0
    Name             0
    Sex              0
    Age            177
    SibSp            0
    Parch            0
    Ticket           0
    Fare             0
    Cabin          687
    Embarked         2
dtype: int64
# Preprocessing complete.
X_train shape: (620, 10)

X_val shape: (155, 10)

Accuracy on validation set: 0.7741935483870968

 # Classification Report:
               precision    recall  f1-score   support

           0       0.79      0.86      0.82        95
           1       0.75      0.63      0.68        60
    accuracy                           0.77       155 
    macro avg      0.77      0.75      0.75       155 
    weighted avg   0.77      0.77      0.77       155


 # Confusion Matrix:
     [[82 13]
     [22 38]]
