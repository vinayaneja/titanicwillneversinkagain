# titanicwillneversinkagain
Kaggle_Titanic_V


data webwork.train;
infile datalines dsd missover;
length PassengerId Survived Pclass Name $ 82;
input PassengerId Survived Pclass Name $ Sex $ Age SibSp Parch Ticket $ Fare Cabin $ Embarked $;
datalines;


# Proc Import

Proc Import Datafile = "location"
Out = Tem_Data
DBMS = csv
Run;
