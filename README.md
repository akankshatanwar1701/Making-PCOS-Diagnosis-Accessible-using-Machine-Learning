# Making PCOS Diagnosis Accessible using Machine Learning: A Quick Summary of What We Have Been Upto!
--------------------------------------------

Polycystic Ovary Syndrome is one of the most common reasons for female infertility. Women with PCOS are often insulin resistant, their body can make insulin but can’t use it effectively, which multiplies the risk of diabetes in them. They also have higher levels of androgens (male hormones that females also have), which can stop eggs from being released (ovulation) and cause irregular periods, acne, thinning scalp hair, and excess hair growth on the face and body.  
  
Polycystic Ovary Syndrome (PCOS) is very common, but it remains undiagnosed and unmanaged in most people who have it. It may affect roughly 1 in 12 women and people with cycles of reproductive age (8%, or ~6-13%), but this likely varies across populations (1-5). Of those who have it, about 7 in 10 may go undiagnosed. (1,2)
  
## Exploratory Analysis 
----------------------------------------------
  
Here, figuring out some parameters which are easily measurable at home and are less invasive becomes a crucial part of our research. Not only the features should be easily measurable but should have a high correlation with diagnostic accuracy.
  
We performed feature selection to find the important attributes to detect PCOS. In order to do that we are using a Kaggle dataset of 541 data points with 41 attributes like Weight Gain, Follicles in the left/Right ovary, LHS levels, Hair loss, BMI, Pimples etc. It is important to note here, **due to very limited prior research** being done in this field it becomes increasingly hard to obtain multiple datasets.  
  
After the pre-processing step of the dataset, the following methods were used to understand the most relevant features:

* Chi-Square Method  
* Correlation Matrix  
* Extra Tree Classifier  

### Chi-Square Method
-------------------------

![alt text](https://github.com/akankshatanwar1701/Making-PCOS-Diagnosis-Accessible-using-Machine-Learning/blob/main/src/Screenshot%20(460).png "Top 20 Features using Chi-Square Method")  
  
### Extra Tree Classifier
-------------------------
  
![alt text](https://github.com/akankshatanwar1701/Making-PCOS-Diagnosis-Accessible-using-Machine-Learning/blob/main/src/Screenshot%20(461).png "Top Top 20 Features using ETC")

### Correlation Matrix
-------------------------

After plotting the heat map, the following features were were closely related to the target feature, arranged in descending order:

* Follicle L and Follicle R
* Skin Darkening
* Hair growth
* Weight Gain
* Cycle (R/I)
* Fast Food 
* Pimples
* AMH levels
* Weight
* BMI 
  
-----------------
After using 3 different statistical methods to pick out the best features that can be used for the detection of PCOS easily, the most overlapping and significant ones can be listed as below:  
  
**Skin Darkening**   
**Hair Growth**   
**Weight Gain**  
**Cycle (R/I)**  
**Pimples**  
  
---------------------

### What Next?

* Currently working on experimenting with various models on the above selected features to get the best maximum accuracy.      
* Building a web-app, which is accessible, easy to use and can be treated as a safe at home tool for PCOS pre-diagnosis, until proper medical care can be provided. 
* Hosting the web-app on Heroku!   
    
![alt text](https://github.com/akankshatanwar1701/Making-PCOS-Diagnosis-Accessible-using-Machine-Learning/blob/main/src/Screenshot%20(462).png "Web App")

## References  
----------------------------
  
1. Bozdag G, Mumusoglu S, Zengin D, Karabulut E, Yildiz BO. The prevalence and phenotypic features of polycystic ovary syndrome: a systematic review and meta-analysis. Human Reproduction. 2016 Nov 17;31(12):2841-55.

2. Broekmans FJ, Knauff EA, Valkenburg O, Laven JS, Eijkemans MJ, Fauser BC. PCOS according to the Rotterdam consensus criteria: change in prevalence among WHO‐II anovulation and association with metabolic factors. BJOG: An International Journal of Obstetrics & Gynaecology. 2006 Oct 1;113(10):1210-7.

3. Christensen SB, Black MH, Smith N, Martinez MM, Jacobsen SJ, Porter AH, et al. Prevalence of polycystic ovary syndrome in adolescents. Fertil Steril. 2013;100(2):470-7.

4. Boyle J, Teede HJ. Polycystic ovary syndrome - an update. Aust Fam Physician. 2012;41(10):752-6.

5. March WA, Moore VM, Willson KJ, Phillips DI, Norman RJ, Davies MJ. The prevalence of polycystic ovary syndrome in a community sample assessed under contrasting diagnostic criteria. Hum Reprod. 2010;25(2):544-51.

6. Sharif E, Rahman S, Zia Y, Rizk NM. The frequency of polycystic ovary syndrome in young reproductive females in Qatar. International journal of women's health. 2017;9:1.

