# Big-Data-Analytics-in-Healthcare
###Modeling and Analysis,Data and Computing,Health Business Context and Problem Solving by
###hands-on experience with scalable machine learning algorithms, big data systems and healthcare data analytic applications

## Goals 
* understanding health care data,
* understanding different analytics algorithms
* understanding big data systems.
* to build models on health care data,example, models for individual disease risk prediction, recommending treatments,
* cluster patient into groups with common characteristics, and find similar patients.

## Problem 
* Healthcare industry is huge. There are a lot of data coming out of healthcare.
* High waste and low quality > 750 billion
* errors and Preventable deaths > 400000

## Health Systems Without Big Data

Most health systems can do plenty today without big data, including meeting most of their analytics and reporting needs.
“air and water” right now (regulatory reporting and operational dashboards), once basic needs are met and some of the initial advanced applications are in place, new use cases can be identifyed in ares of big data. 

## Barriers
* Technical expertise(most organizations need data scientists/data engineers to manipulate and get data out of a big data environment), curruntly only limited to research because of complexity 

* Security : In healthcare, HIPAA compliance is non-negotiable. Nothing is more important than the privacy and security of patient data. 

* Funding 

* Governance and Policy 

## Big data concepts 

### Big Data Has Minimal Structure
Compared to classical relation data bases, where data is stored in schema and linked to different identifiers.Here data has hardly any structure at all. Data is extracted from source systems in its raw form stored in a massive distributed file system.

### four Vs

* Volume- Health generates large amount of data For example, for genomic data each human genome requires 200 gigabyte of raw data, or 125 megabyte if we store just snipps. For medical imaging data a single FMRI is about 300 gigabyte.
Medical imaging data generated in the US per year was estimated to be 100 petabyte.
Healthcare also generates lots of different kinds of information such as clinical informations, including patients demographics, diagnosis, procedure, medication, lab results, and clinical notes.
And patient generated data, such as the information coming out of on-body sensors and other devices that patients wear.
And real-time data sources such as blood pressure measures, temperature, heart rate, drug dispensing levels at intensive care units.

* Varity- sensors/twitter/facebook/etc

* Varecity - Veracity, there's a common problem with the veracity,there's lot of noise, lot of missing data, lot of errors,
and a lot of false alarms.

* velocity - real time data

## Big Data Picture

* Big data systems
* Machine learning Algorithims
* Healthcare Applications

### Healthcare Applications

Three types ....
* Predective Modeling -- to predict future outcome e.g epilepsy - (will help in matching patient to right treatment) 
* Computational Phenotyping -- turning massive EHR to meaning full health concepts 
* Patient Similarity --- to identify group of patients based on similar characteristics  


#### Predective Modeling
Why difficult ? We have millions of patients we want to analyze and their diagnosis information, medication information, and so on. So all those data combined together, create a big challenge. The second challenge in predictive modeling is there are so
many models to be built. Predictive model is not a single algorithm, it's a sequence of computational tasks. Which can be described as Predective modelling pipline. 100000 different piplines can be developed.

start --- cohort construction --- feature construction --- cross validation --- feature selection -- classification -- output


#### Computational Phenotyping

The input to Computational Phenotyping is the raw patient data. It consist of many different sources, such as demographic information, diagnosis, medication, procedure, lab tests, and clinical notes. And phenotyping is the process of turning the raw
patient data into medical concepts or phenotypes.

Raw Data ---- phenotypying ---- to Medical Concepts 

to extract phenotypes we deal with missig data , redudency , duplication , irrevelent data e.g For example, post diagnosis and
medication records from a patient indicate underlying condition of type 2 diabetes. So we want to consolidate those redundant informatio

EHR ---type 1 diebeties diagnosis  --- No ----- Type 2 dibeties diagnosis ---- no type 2 treatment --- yes abnormal lab ---- case 

type 2 diagnosis yes --- type 1 treatment no --- type 2 treatment no ---- abnormal lab ----  yes type 2 dibeties 

why complex algorithim ? The reason is because electronic health record data is very unreliable.
There are missing data, redundant information, so sometimes for Type 2 diabetes patients, the diagnosis is not present in the record. So we still have other ways to check whether they are a Type 2 diabetes patient, for example, their medication, lab test.

#### Patient Similarity 

