# Bank's classifier
## Table of contents
* [General info](#general-info)
* [Features](#features)
* [Process](#process)
* [Stack](#stack)
* [Conclusion](#conclusion)

## General info
This project is made for classification of ouflow of clients in telecommunications.
Question arises: what features can help us to understand whether person leaves or stays
## Features
- customerID — идентификатор абонента
- BeginDate — дата начала действия договора
- EndDate — дата окончания действия договора
- Type — тип оплаты: раз в год-два или ежемесячно
- PaperlessBilling — электронный расчётный лист
- PaymentMethod — тип платежа
- MonthlyCharges — расходы за месяц
- TotalCharges — общие расходы абонента
- customerID — идентификатор пользователя
- gender — пол
- SeniorCitizen — является ли абонент пенсионером
- Partner — есть ли у абонента супруг или супруга
- Dependents — есть ли у абонента дети
- customerID — идентификатор пользователя
- InternetService — тип подключения
- OnlineSecurity — блокировка опасных сайтов
- OnlineBackup — облачное хранилище файлов для резервного копирования данных
- DeviceProtection — антивирус
- TechSupport — выделенная линия технической поддержки
- StreamingTV — стриминговое телевидение
- StreamingMovies — каталог фильмов
- customerID — идентификатор пользователя
- MultipleLines — подключение телефона к нескольким линиям одновременно
## Process
|Stage | Description|
|--------|--------|
|First stage| Data analysis of each dataset: trying to understand how to merge in order to get more customers|
|Second stage|Merging data and checking for disblance,creating target|
|Third stage|Inroducing new features and checking them for correlation with target|
|Fourth stage|Eliminating features that create little to no explanation of target|
|Fifth stage|Plotting plots for data distribution|
|Sixth stage|Data division into training and test|
|Seventh stage|Setting up pipelines for models RandomizedSearchCV|
|Eighth stage|After we found the best parameters for the best model,we can finally use it on test data|
|Nineth stage|The auc_roc is high enough(93%): now we can find out features importance and presenet reccomendation for business|

## Stack
Project is created with:
* Pandas
* Sklearn
* Numpy
* Matplotlib.pyplot
* Shap
* Catboost
* Seaborn
	
## Conclusion
There is a strong correlation between the atrget and the amount of months that are spent on service,also provider shouldn't ignore special deals for customers that pay more
The result is good score and 92% accuracy



