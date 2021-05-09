## Table of Contents
- [Goal](#blog)
- [Prerequisites](#prerequisites)
- [Data](#data)
- [Processing](#Processing)
- [Results](#results)
- [License](#license)

<br>

## Goal
 * Prioritization of partner's countries based on health-related indicators
 

<br>

## Prerequisites
 * Install Python 3
 * Install dependencies 

```bash 
cd SWB165
pip install -r src/requirements.txt 
```
<br>

## 1. Data 
### 1.1 Partner's Data 
 * Three lists of countries from 2018-2020

### 1.2 WHO Data
#### 1.2.1 Country Code Data 
#### 1.2.2 Indicator Code
#### 1.2.3 Indicator Data with Different Dimensions 
 * Country
 * Regional 
 * Time 

<br>

## 2. Processing
### 2.1 Partner's Data 
#### 2.1.1 Merge Data 
#### 2.1.2 Clean Data 


### 2.2 Process WHO Data
#### 2.2.1 Country Code
 * Download data

#### 2.2.2 Merge WHO Country Code with Partner's Country Names
   * Exact match of country names
   * Fuzzy match of country names 
     * Remove wrong match from multiple fuzzy matches
   * Remove countries with the same country code

#### 2.2.3 Indicator Code 
 * Download data

#### 2.2.4 Indicator Data 
 * Download data
 
#### 2.2.5 1st Filter of Indicator Data using Partner's Country Condition 
 * Input: 2.2.4 
 * Condition: 2.2.2  

#### 2.2.6  Summarize Indicator Data 
 * Group by Indicator Code
   * Summarize the number of Partner's countries 
   * Summarize the number of Time Dimensions (Year)

#### 2.2.7 2nd Filter of Indicator Data 
 * Input: 2.2.5 
 * Condition: 2.2.6 

#### 2.2.8 Merge all Indicator Data  

#### 2.2.9 Classification of Indicators
 * Positive
 * Negative 

<br>

## 3. Results

### 3.1 Clustering
#### 3.1.1 Hierarchy Clustering using Dendrogram
  * Tool: SPSS 

#### 3.1.2 Visualization 
 * PCA
 * t-SNE  

### 3.2 Ranking 
 



<br>


## License 

