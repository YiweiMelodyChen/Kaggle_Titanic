# Kaggle_Titanic

## Decision Tree
followed by https://www.kaggle.com/nedaamiri/titanic-decision-tree.

Used packages are as follows

### DataFrame Package

**pd.read_csv**: read .csv file 

**df.head**

**df.info()**: abstract of the dataframe

**df.describe()**: the statistical info about the df

**df.shape**

**df['columns'].value_counts()**: count the distribution of each column

**df.isnull()**

**df.drop()** df_train.drop('Cabin', axis=1, inplace=True)

**df.loc** df_train.loc[df_train['Sex']=='male', 'Sex']=1

**df.fillna()** df_train['Age'].fillna(df_train['Age'].mean(), inplace=True)

### Plot Package

**sns.countplot** (data=df_train, x='Survived')  

**sns.heatmap** (df_train.corr(), annot=True, cmap='winter')

### Model Package

**sklearn.model_selection.train_test_split**  
split the dataset to train and validation set

**sklearn.preprocessing.StandardScaler** scale the data

**sklearn.tree.DecisionTreeClassifier** 
max_depth, max_leaf_nodes, criterion

**from sklearn.metrics import classification_report, confusion_matrix**

**model.feature_importances_**

**sklearn.tree.plot_tree**

