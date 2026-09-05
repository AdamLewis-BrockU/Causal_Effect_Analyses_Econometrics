# Causal_Effect_Analyses_Econometrics
Created by Adam Lewis. Includes jupyter notebooks (.ipynb files) written in python and markdown.


---


# **<u> Abortion_CEA.ipynb File </u>**

### **Dataset Used:**

https://osf.io/k4x7t/files/kqb9n - Link to Dataset

https://www.guttmacher.org/monthly-abortion-provision-study?state=US - Parent Website

### **Dataset Description:**

**Title:** Monthly Abortion Provision Study

**Description:** The Monthly Abortion Provision Study (https://www.guttmacher.org/monthly-abortion-provision-study) produces national and state estimates of the number of abortions provided in states without total bans in the United States. This ongoing project reveals current trends and aims to put timely data in the hands of policymakers, advocates and providers. Details on how to access project files and citation information can be found in Wiki below,

**Date created:** August 31, 2023

**Date modified:** July 21, 2026

**Contributors:** Isaac Maddow-Zimet, Isabel DoCampo, Rachel Jones, Ava Braccia, Mariah Menanno, Aisiri Murulidhar, Priscille Osias, Lauren Mitchell, Jesse Philbin

### **Problem to be Answered:**
- Do abortion restrictions cause a decrease in number of abortions?


---


# **<u> CoffeeHealth_CEA.ipynb File </u>**

### **Dataset Used:**

https://www.kaggle.com/datasets/uom190346a/global-coffee-health-dataset

### **Dataset Description:**

**Global Coffee Health Dataset**

**Description:** The GlobalCoffeeHealth dataset contains 10,000 synthetic records reflecting real-world patterns of coffee consumption, sleep behavior, and health outcomes across 20 countries. It includes demographics, daily coffee intake, caffeine levels, sleep duration and quality, BMI, heart rate, stress, physical activity, health issues, occupation, smoking, and alcohol consumption. The dataset captures realistic correlations observed in research—such as caffeine’s impact on sleep, stress, and health—making it ideal for statistical analysis, predictive modeling, and lifestyle or wellness studies.

![image.png](attachment:image.png)

### **Problem to be Answered:**
- Does an increase in coffee consumption cause an increase in heart rate?
- A higher heart rate is related to overall health. 
- Typically a person who has high heart rate also has worse health and heart related problems since the heart must work harder.


---


# **<u> DID.ipynb </u>**

### **Card & Krueger (1994) Difference-in-Difference Causal Analysis**

### **Context:**
"On April 1, 1992, New Jersey's minimum wage rose from $4.25 to $5.05 per hour. To evaluate the impact of the law we surveyed 410 fast-food restaurants in New Jersey and eastern Pennsylvania before and after the rise. Comparisons of employment growth at stores in New Jersey and Pennsylvania (where the minimum wage was constant) provide simple estimates of the effect of the higher minimum wage. We also compare employment changes at stores in New Jersey that were initially paying high wages (above $5) to the changes at lower-wage stores. We find no indication that the rise in the minimum wage reduced employment" (David Card and Alan B. Krueger).

### **Links:**

https://davidcard.berkeley.edu/papers/njmin-aer.pdf?utm_source=chatgpt.com

https://davidcard.berkeley.edu/data_sets.html?utm_source=chatgpt.com

**Simplified Dataset Used:** https://www.ssc.wisc.edu/~bhansen/econometrics/CK1994.dta?utm_source=chatgpt.com 

### **Description:**

![image.png](attachment:image.png)

![image-2.png](attachment:image-2.png)

### **Columns:**
1) state
    - 1 = New Jersey.
    - 0 = Pennsylvania.
2) empft
    - Number of full-time employees.
3) emppt
    - Number of part-time employees.
4) nmgrs
    - Number of managers.
5) time
    - 1 = After the minimum wage increase from $4.25 to $5.05 per hour.
    - 0 = Before the minimum wage increase from $4.25 to $5.05 per hour.

### **Problem to be Answered:**
- Difference in Difference (DID) Design Causal Analysis.


---


# <u> EstimatedCausalEffects.ipynb File </u>**

## <u> **1) Education and Earnings: Does more education cause an increase in earnings?** </u>

### **Dataset Used:**

https://vincentarelbundock.github.io/Rdatasets/csv/wooldridge/wage1.csv?utm_source=chatgpt.com 

https://vincentarelbundock.github.io/Rdatasets/doc/wooldridge/wage1.html?utm_source=chatgpt.com

### **Dataset Description:**

Wooldridge Source: These are data from the 1976 Current Population Survey, collected by Henry Farber when he and I were colleagues at MIT in 1988.

A dataframe with 526 observations on 24 variables:
- wage: average hourly earnings
- educ: years of education
- exper: years potential experience
- tenure: years with current employer
- nonwhite: =1 if nonwhite
- female: =1 if female
- married: =1 if married
- numdep: number of dependents
- smsa: =1 if live in SMSA
- northcen: =1 if live in north central U.S
- south: =1 if live in southern region
- west: =1 if live in western region
- construc: =1 if work in construc. indus.
- ndurman: =1 if in nondur. manuf. indus.
- trcommpu: =1 if in trans, commun, pub ut
- trade: =1 if in wholesale or retail
- services: =1 if in services indus.
- profserv: =1 if in prof. serv. indus.
- profocc: =1 if in profess. occupation
- clerocc: =1 if in clerical occupation
- servocc: =1 if in service occupation
- lwage: log(wage)
- expersq: exper^2
- tenursq: tenure^2

### **Problem to be Answered:**
- Does more education cause an increase in earnings?

## <u> **2) Smoking and Birth Weight: Does smoking during pragnancy cause a decrease in baby birth weight?** </u>

### **Dataset Used:**

https://www.kaggle.com/datasets/jacopoferretti/child-weight-at-birth-and-gestation-details 

### **Dataset Description:**

The dataset provides information on a child's weight at birth plus some stats on the child's mother: is she a smoker or not, her height, her weight, the gestation length, and so on

A dataframe with 1236 observations on 8 variables:
- case: Index for each sample, 0 to 1235.
- bwt: Birth weight of baby in ounces (oz).
- gestation: Days fetus spent in womb.
- parity: The number of births (including live births and stillbirths) where pregnancies reached viable gestational age. https://en.wikipedia.org/wiki/Gravidity_and_parity 
- age: Age of woman.
- height: Height of woman.
- weight: weight of woman.
- smoke: 1 = Woman smoked during pragnancy, 0 = Woman did not smoke during pragnancy.

### **Problem to be Answered:**
- Does smoking during pragnancy cause a decrease in baby birth weight?

## <u> **3) COVID Lockdowns: Did COVID lockdowns cause a larger decrease in student scores at poorer schools?** </u>

### **Dataset Used:**

https://www.kaggle.com/datasets/dylanbollard/covid19-effect-on-grades-constructed-dataset

### **Dataset Description:**
This dataset was generated in order to fullfill a requirement for a graduate class in applied econometrics. I originally wanted to collect data on the effect of COVID-19 on student performance from a school district, but was unable to given that our local district was already conducting their own research.

The set contains a panel dataset, meant to emulate 6 semesters/trimesters with the first three taking place before the COVID-19 lockdowns, and the final three coming after the lockdowns. It also contains a cross-sectional dataset that is meant to be a single semester/trimester after the COVID-19 lockdowns. Variables were included and manipulated to model real world trends, or local demographics in Portland Oregon. There is a full list of variables at the end of this markdown.

It should be noted that student performance has greatly been diminished as a result of online education.

### **VARIABLES used in the program (NAME DATATYPE PURPOSE):**

### **PERSONAL INFORMATION:**

- studentID into Number assigned to student. 
- school dummy 0/1, bool 1=school B (poor), 0= school A (wealthy)
- gradelevel int Determine grade level of child.
- gender dummy 0/1, bool 1=male, 0=female 
- covidpos dummy 0/1 1=child had Covid, 0=null 
- freelunch dummy 0/1 1=takes free and reduced lunch, 0=null
- timeperiod categorical {0,1,2}=in-person learning, {3,4,5}=online learning 
- numcomputers into Defines number of computers in child's home. 
- familysize int Defines size of family, parents and siblings.
- householdincome float Household income for child. 
- fathereduc categorical System of values for highest level of father education, no HS diploma = 0, High School diploma 1, Highest level of education is High School. Bachelor degre = 2. Master's Degree = 3. Doctoral Degree = 4. Then, if fathereduc = 0, father did not finish High School.
- mothereduc categorical System of values for highest level of mother education, no HS diploma = 0, High School diploma = 1 Highest level of education is High School. Bachelor degre = 2. Master's Degree = 3. Doctoral Degree = 4. Then, if mothereduc = 0, mother did not finish High School. 

### **SCHOOL PERFORMANCE INFORMATION:**
- readingscore float Score for "reading" test in school.
- writingscore float Score for "writing" test in school.
- mathscore float Score for "math" test in school.

### **STATE PERFORMANCE INFORMATION:**
- readingscoreSL float Score for "reading" test at state level.
- writingscoreSL float Score for "writing" test at state level.
- mathscoreSL float Score for "math" test at state level.

### **Problem to be Answered:**
- Did COVID lockdowns cause a larger decrease in student scores at poorer schools?


---


# **<u> EstimatedCausalEffects2.ipynb </u>**

## <u> **1) Memory Test on Drugged Islanders: Does the drug Xanax cause high memory recal after drug is administered?** </u>

### **Dataset Used:**

https://www.kaggle.com/datasets/steveahn/memory-test-on-drugged-islanders-data

### **Dataset Description:**

**Context:**

An experiment on the effects of anti-anxiety medicine on memory recall when being primed with happy or sad memories. The participants were done on novel Islanders whom mimic real-life humans in response to external factors.

Drugs of interest (known-as) [Dosage 1, 2, 3]:

A - Alprazolam (Xanax, Long-term) [1mg/3mg/5mg]

T - Triazolam (Halcion, Short-term) [0.25mg/0.5mg/0.75mg]

S- Sugar Tablet (Placebo) [1 tab/2tabs/3tabs]

*Dosages follow a 1:1 ratio to ensure validity *Happy or Sad memories were primed 10 minutes prior to testing *Participants tested every day for 1 week to mimic addiction

**Building the Case: Obstructive effects of Benzodiazepines (Anti-Anxiety Medicine):** Long term adverse effects on Long Term Potentiation of synapses, metacognition and memory recall ability http://www.jstor.org/stable/43854146

**Happy Memories:** Research shown positive memories to have a deeper and greater volume of striatum representation under an fMRI https://www.sciencedirect.com/science/article/pii/S0896627314008484

**Sad Memories:** Research shown sad memories invokes better memory recall for evolutionary purpose whereas, happy memories are more susceptible to false memories http://www.jstor.org/stable/40064315

**Participants:** All genders above 25+ years old to ensure a fully developed pre-frontal cortex, a region responsible for higher level cognition and memory recall.

**Content:** File contains information on participants drug treatment information along with their test scores.

**Acknowledgements:** Experiment was executed under the supervision of Mr. Almohalwas at UCLA. All aspects of the experiment such as experimental design, data collection and preprocessing was done from the authour Steve Ahn.

### **Problem to be Answered:**
- Does the drug Xanax cause higher memory recal after drug is administered?

## <u> **2) School Lunch Program: Does free lunch at schools cause an improvement in grades?** </u>

### **Dataset Used:**

https://www.kaggle.com/datasets/bhavikjikadara/student-study-performance

### **Dataset Description:**

**Problem Statement:** This project understands how the student's performance (test scores) is affected by other variables such as Gender, Ethnicity, Parental level of education, Lunch and Test preparation course.

**Content:** This data set consists of the marks secured by the students in various subjects.
- gender : sex of students -> (Male/female)
- race/ethnicity : ethnicity of students -> (Group A, B, C, D, and E)
- parental level of education : parents' final education ->(bachelor's degree,some college,master's degree,associate's degree,- high school)
- lunch : having lunch before test (standard or free/reduced)
- test preparation course : complete or not complete before test
- math score
- reading score
- writing score

**Inspiration:** To understand the influence of the parent's background, test preparation etc on students' performance

### **Problem to be Answered:**
- Does free lunch at schools cause an improvement in grades?

## <u> **3) Caffeine Intake: Does the amount of coffee consumed cause more energy?** </u>

### **Dataset Used:**

https://www.kaggle.com/datasets/uom190346a/global-coffee-health-dataset

### **Dataset Description:**

**Global Coffee Health Dataset**

**Description:** 

The GlobalCoffeeHealth dataset contains 10,000 synthetic records reflecting real-world patterns of coffee consumption, sleep behavior, and health outcomes across 20 countries. It includes demographics, daily coffee intake, caffeine levels, sleep duration and quality, BMI, heart rate, stress, physical activity, health issues, occupation, smoking, and alcohol consumption.

The dataset captures realistic correlations observed in research—such as caffeine’s impact on sleep, stress, and health—making it ideal for statistical analysis, predictive modeling, and lifestyle or wellness studies.

![image.png](attachment:image.png)

**Usage & Insights:**
- Explore correlations between coffee intake, sleep quality, and health outcomes.
- Analyze lifestyle factors like physical activity, smoking, and alcohol consumption.
- Build predictive models for sleep quality, stress levels, or health risks.
- Compare demographic and country-level patterns in caffeine consumption.
- Use as a benchmark dataset for wellness, lifestyle, or health informatics research.

### **Problem to be Answered:**
- Does mode coffee cause less hours of sleep?


---


# **<u> Guns_CEA.ipynb </u>**

### **Dataset Used:**

https://www.kaggle.com/datasets/ahmedeltom/us-gun-deaths-by-county-19992019

### **Dataset Description:**

The dataset is sourced and edited from
data.world

Description is given as below:

Centers for Disease Control and Prevention, National Center for Health Statistics. Multiple Cause of Death with U.S. - Mexico Border Regions 1999-2019 on CDC WONDER Online Database, released in 2020. Data are from the Multiple Cause of Death Files, 1999-2019, as compiled from data provided by the 57 vital statistics jurisdictions through the Vital Statistics Cooperative Program. U.S. - Mexico border counties has been demarcated as the 44 counties that are located within 100 kilometers (62 miles) defined under the 1983 La Paz Agreement. Accessed at http://wonder.cdc.gov/ucd-border.html on Nov 6, 2021 12:22:30 AM

Query Parameters: Title: Gun Deaths by County MCD - ICD-10 Codes: W32 (Handgun discharge); W33 (Rifle, shotgun and larger firearm discharge); W34 (Discharge from other and unspecified firearms); X72 (Intentional self-harm by handgun discharge); X73 (Intentional self-harm by rifle, shotgun and larger firearm discharge); X74 (Intentional self-harm by other and unspecified firearm discharge); X93 (Assault by handgun discharge); X94 (Assault by rifle, shotgun and larger firearm discharge); X95 (Assault by other and unspecified firearm discharge); Y22 (Handgun discharge, undetermined intent); Y23 (Rifle, shotgun and larger firearm discharge, undetermined intent); Y24 (Other and unspecified firearm discharge, undetermined intent); Y35.0 (Legal intervention involving firearm discharge)

Group By: Year; County Show Totals: True Show Zero Values: False Show Suppressed: False Standard Population: 2000 U.S. Std. Population Calculate Rates Per: 100,000 Rate Options: Default intercensal populations for years 2001-2009 (except Infant Age Groups)

picture sourced from peterplit

### **Problem to be Answered:**
- Do gun laws and restrictions cause a decrease in gun related deaths per US county?


---


# **<u> SocialMedia_CEA.ipynb File </u>**

### **Dataset Used:**

https://www.kaggle.com/datasets/muqniturrehman/social-media-and-academic-performance-of-students

### **Dataset Description:**
- Unfortunatly, there is no description given for this dataset on kaggle.
- So, we will assume that the sample of college/university students was collected randomly.
- Random sampling did in fact take place, but as for the treatment we will assume it was not assigned at random.
- The students choose to interact with social media on their own terms, for however long they wanted.

### **Problem to be Answered:**
- Does an increase in hours spent on social media cause a decrease in academic performance GPA?

