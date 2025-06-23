Code Explaination

Data Preparation & Cleaning

1. Mount Google Drive: Allows access to files stored in the user's Google Drive.


2. Import Libraries: Loads packages like pandas, numpy, seaborn, and matplotlib for data manipulation and visualization.


3. Load Dataset: Reads the Titanic dataset CSV file from Drive into a DataFrame.


4. Basic Info & Missing Values: Displays data types and counts of missing values for each column.


5. Handle Missing Data:

Age: Filled with median.

Embarked: Filled with mode.

Fare: Filled with median.




Feature Engineering

6. Family Size: Combines SibSp and Parch to form a new feature indicating family size.


7. IsAlone: A binary feature indicating if a passenger was alone.


8. Title Extraction:

Extracts titles from the Name column.

Replaces rare titles with 'Rare'.

Maps equivalent titles (e.g., Mme → Mrs).

Encodes titles into numeric format.




Encoding & Transformation

9. Encode Categorical Variables:

Sex: Male = 0, Female = 1.

Embarked: C = 0, Q = 1, S = 2.



10. Drop Unnecessary Columns: Removes PassengerId, Name, Ticket, and Cabin.



Normalization & Outlier Removal

11. Standardize Numeric Features: Scales Age, Fare, and FamilySize using StandardScaler.


12. Remove Outliers in Fare: Uses IQR method to remove extreme values in Fare.



Modeling

13. Split Data: Divides the dataset into training and validation sets (80% / 20%).


14. Train Model: Trains a logistic regression model on the training data.


15. Evaluate Model:



Predicts on validation data.

Displays accuracy, classification report, and confusion matrix.


Visualization

16. Boxplots (Before Outlier Removal): Visualizes distributions of Age, Fare, and FamilySize before removing outliers.


17. Custom Function for Outlier Removal: Reusable function to remove outliers from any numeric column.


18. Apply to All Numeric Columns: Removes outliers from Age, Fare, and FamilySize.


19. Boxplots (After Outlier Removal): Shows how the data looks after outliers are removed.
