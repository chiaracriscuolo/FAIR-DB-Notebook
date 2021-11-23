# FAIR-DB-Notebook
Python notebooks of FAIR-DB system (a framework to detect biases and discover discrimination in datasets) with two input datasets (Titanic and Adult Census U.S.) The python notebooks present FAIR-DB workflow applied to one dataset at a time. Try with your own dataset and input parameters to discover bias and unfairness in your custom dataset!

## Paper Abstract
Computers and algorithms have become essential tools that pervade all aspects of our daily lives; this technology is based on data and, for it to be reliable, we have to make sure that the data on which it is based on is fair and without bias. In this context, Fairness has become a relevant topic of discussion within the field of Data Science Ethics, and in general in Data Science. Today’s applications should therefore be associated with tools to discover bias in data, in order to avoid (possibly unintentional) unethical behavior and consequences; as a result, technologies that accurately discover discrimination and bias in
databases are of paramount importance.
In this work we propose FAIR-DB (FunctionAl dependencIes to discoveR Data Bias), a novel solution to detect biases and discover discrimination in datasets, that exploits the notion of Functional Dependency, a particular type of constraint on the data. The proposed solution is implemented as a framework that focuses on the mining of such dependencies, also proposing some new metrics for evaluating the bias found in the input dataset. Our tool can identify the attributes of the database that encompass discrimination (e.g. gender, ethnicity or religion) and the ones that instead verify various fairness measures; moreover, based on special aspects of these metrics and the intrinsic nature of dependencies, the framework provides very precise information about the groups treated unequally, obtaining more insights regarding the bias present in dataset compared to other existing tools. Finally, our system also suggests possible future steps, by indicating the most appropriate (already existing) algorithms to correct the dataset on the basis of the computed results.

Link: http://ceur-ws.org/Vol-2841/PIE+Q_4.pdf , http://ceur-ws.org/Vol-2994/paper19.pdf

## Start Guide

The algorithm needs an external system to extract the Functional Dependencies (https://github.com/j-r77/cfddiscovery). Make sure to compile it with cmake and put the dataset in .csv format in its "dataset" folder. 

FAIR-DB takes as inputs:
- The dataset in csv format
- The protected attributes 
- The target class
- The minimum support threshold
- The confidence leeway threshold
- The maximum antecedent size of the discovered CFDs
- The Difference minimum threshold.
