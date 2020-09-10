# Python
**Requirement**

  1. Write a script in PySpark to read in the data. Ensure that you will only be working with the Trade Type “Standard”.
  2. Add a couple of features to the dataset:     The expected duration: the number of days between advance date and expected 
  payment date.     The number of previously settled trades for the seller. Make sure to only count trades where the Settlement Date is before the Advance Date of the trade.
  3. Don't use any external library, but try to solve the problem with the normal functionality. 

**Python NotebookName**

    LoanBookTranformation.ipynb

This note book contains spark commands to 

    1.Read the xml files and build the data frame
    2.Appply the transformations according to the requirements
    3.Two cloumns **expected_duration, previous_settled_trade_cont** has been added with the the necessary logic
 
**Observations**

    Most of the data does come under the scenario settlement_date > advance_date.
    To fulfil the second requirement,Data Modification is required.Hence above condition is used

**Scope for Improvements**

     Quality checks
     Logging
     Converting into Object oriented code,modules
     Reading/parsing xml will be eaiser with the external library com.databricks:spark-xml_2.10:0.4.1


**For Test the skills of a Data Engineer**

      The current task would be a good start to test skills of data engineer since it has all the aspects of Reading,parsing and transforming the data
      It is better to have final destination (hdfs/cloud storage) to load the data,since it covers extract,transform 

**Note**

To view the notebook please open in jupyter notebook OR can see here in github directly along with the results
