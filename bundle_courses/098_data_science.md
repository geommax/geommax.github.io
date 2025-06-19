# Statistics Course Modules
*[Home](../README.md),  [Training Materials](../trainingmaterials.md),  [Github](https://github.com/ROM-robotics),  [Popular Bundle Courses](../bundle_courses.md)*
## About
> Data Analysis လုပ်ချင်တဲ့သူတွေတွက်ပဲဖြစ်ပါတယ်။


> Statistics က Robotics Engineering မှာ ဘယ်လောက်အရေးပါသလဲ? ဘယ်လိုအသုံးပြုသလဲ?


Statistical methods တွေက robotics engineering နယ်ပယ်မှာ အခြေခံကျတဲ့ဘာသာရပ်တစ်ခုဖြစ်ပြီးတကယ့် robotic system ထဲမှာရှိတဲ့ မသေချာမှုတွေ variability တွေနဲ့ noise တွေကိုကိုင်တွယ်ဖို့အတွက်အဓိက ထောက်ပံ့ပေးတဲ့ပညာရပ်တစ်ခုဖြစ်ပါတယ်။


### 1. Handling Uncertainty (မသေချာမှုကိုကိုင်တွယ်ခြင်း)

ကြိုတင်ခန့်မှန်းလို့မရတဲ့ environments တွေမှာ robotics system လည်ပတ်တဲ့အခါ
* Sensor ဖတ်တဲ့အခါ noisy တွေ မပြည့်စုံမှုတွေပါလာခြင်း။
* Actuator (ထိန်းကျောင်းကိရိယာ) လှုပ်ရှားမှုက မျှော်မှန်းထားသောအခြေအနေကနေသွေဖယ်ခြင်း။
* ကျပန်းဖြစ်ပေါ်နေတဲ့ (wealther, lighting, obstacles) တွေလို external factors များသက်ရောက်မှုရှိခြင်း။
Solving problem with Statistical role
Probabilities models တွေဖြစ်တဲ့ Bayesian networks လိုကောင်မျိုးတွေက မသေချာမှုတွေကိုတိုင်းတာပြီး ရှုပ်ထွေးပြီးမပြည့်စုံတဲ့ data တွေကို robots တွေကဆုံးဖြတ်ချက်ချတဲ့အခါ အကူညီပေးပါတယ်။ ဥပမာ self driving car တွေမှာဆိုရင် မရွေ့လျားတဲ့အဟန့်အတားခလုပ်ကန်သင်းတွေရဲ့ probability ကိုခန့်မှန်းဖို့အတွက် Statistical methods တွေကိုအသုံးပြုပါတယ်။


### 2. Sensor Fusion (Sensor ပေါင်းစပ်ခြင်း)

Modern robots တွေက သူတို့ရဲ့ environment ကိုသိမြင်နားလည်ဖို့ cameras, lidar, GPS နဲ့ IMUs လို multiple sensors တွေကို အားကိုးရပါတယ်။ Sensor အသီးသီးက noisy တွေ တစ်ခါတစ်ရံဝိရောဓိဖြစ်စရာ data တွေကိုကိုင်တွယ်ဖို့ထောက်ပံ့ပေးပါတယ်။
Solving problem with Statistical role
Kalman filters တို့ Bayesian fusion တို့က robots ကျင်လည်မယ့် environment နဲ့လိုက်လျောညီထွေဖြစ်ဖို့ ပိုမိုတိကျတဲ့ result တွေရဖို့ဖနိတီးတဲ့အခါ data တွေကိုပေါင်းစပ်ဖို့ကူညီပေးပါတယ်။ ဥပမာ Autonomous drones တွေမှာ accelerometer data နဲ့ merging GPS က တည်ငြိမ်စွာပျံသန်းနိုင်ဖို့ sensor fusuion ကိုအသုံးပြုပါတယ်။

### 3. Localization & Mapping

Simultaneous localization နဲ့ mapping (SLAM) က robotics ရဲ့အဓိက ဗဟိုချက်ပြဿနာတစ်ခုဖြစ်ပါတယ်။ 

* Unknown environment မှာသူရဲ့ position ကိုနားလည်ဖို့။
* Environment ရဲ့ map ကိုဖန်တီးဖို့ စတာတွေကအဓိက ပြဿနာနဲ့လိုအပ်ချက်ဖြစ်ပါတယ်။

Solving problem with Statistical role

Probabilistic models တွေဖြစ်တဲ့ particle filters, Gaussian process လို method တွေက motion နဲ့ sensor data ထဲက မရေရာမှုတွေရဲ့ အသေးစိတ်ဖြစ်ရပ်ကိုဖော်ပြပေးပါတယ်။ ဥပမာ Roomba နဲ့ တခြားသော autonomous vacuums တွေက rooms တွေကို map လုပ်ဖို့နဲ့လမ်းညွန်အတိုင်းမောင်းနှင်နိုင်ဖို့ SLAM algorithms တွေကိုသုံးပါတယ်။

### 4. Robot Perception

Robot တွေက သူတို့ရဲ့ environment ကိုသိမြင်နားလည်ဖို့ images, sound နဲ့ sensor data တွေကို သုံးပါတယ်။ ဒါပေမယ့် ထို data တွေက noisy တွေ မရှင်းလင်းမှုတွေက မူရင်းထဲကပါလာတက်ပါတယ်။

Solving problem with Statistical role

Computer vision system တစ်ခုမှာ Hidden Markov Models (HMMs) , Convolutional Neural Networks (CNNs) နဲ့ Bayesian inference တို့လို Statistical methods တွေကိုပါသုံးပါတယ်။ ဥပမာ Tesla ရဲ့ autopilot identifies objects က car တွေ လမ်းသွားလမ်းလာလူတွေကို statistical classification နဲ့ pattern recognition နဲ့ real time classification လုပ်ပါတယ်။

### 5. Decision - Making & Path Planning

Robot တွေက complex နဲ့ dynamic environments မှာ မပြည့်စုံတဲ့ information တွေနဲ့ အတူ decision making လုပ်ဖို့လိုအပ်ပါတယ်။

Solving problem with Statistical role

Decision making frameworks တွေဖြစ်တဲ့ Markov Decision Processes (MDPs) နဲ့ reinforcement learning က robots ရဲ့ weight probabilities တွက်ချက်ဖို့နဲ့ optimal actions တွေကို ရွေးချယ်ဖို့ကူညီပေးပါတယ်။ ဥပမာ Starship လို delivery robots တွေက statistical optimization ကိုအသုံးပြုပြီး အတားအဆီးတွေ ရှောင်ကွင်းပြီး သင့်တော်တဲ့လမ်းကြောင်းကိုရွေးချယ်ရွေ့လျားကြပါတယ်။

နောက်ထပ်လည်း Robotics Engineering မှာ Statistical methods တွေကို ဘယ်လိုအသုံးချပြီး တည်ဆောက်နေကြသလဲဆိုတာကိုထပ်မံ sharing လုပ်ပေးသွားပါမယ်။


> Kyaw Kyaw Htut (Ace Of Data)


## Module - 1: Nature of Statistics
- **Descriptive & Inferential Statistics**
- **Variables and Data Types**
- **Data Collection and Sampling Techniques**
- **Experimental Design**

## Module - 2: Frequency Distribution
- **Organizing Data with Frequency Distribution**
- **Histogram, Frequency Polygons, and Ogives**
- **Types of Graphs**

## Module - 3: Data Description
- **Measure of Central Tendency**
- **Measure of Variation**
- **Measure of Position**
- **Exploratory Data Analysis**

## Module - 4: Probability and Counting Rules
- **Sample Spaces and Probability**
- **The Addition Rules for Probability**
- **The Multiplication Rules and Conditional Probability**
- **Counting Rules**
- **Probability and Counting Rules**

## Module - 5: Discrete Probability Distributions
- **Probability Distributions**
- **Mean, Variance, Standard Deviation, and Expectation**
- **The Binomial Distribution**
- **Types of Distributions**

## Module - 6: The Normal Distribution
- **Normal Distribution**
- **Applications of the Normal Distribution**
- **The Central Limit Theorem**
- **The Normal Approximation to the Binomial Distribution**

## Module - 7: Confidence Intervals and Sample Size
- **Confidence Intervals for the Mean when Sigma is Known**
- **Confidence Intervals for the Mean when Sigma is Unknown**
- **Confidence Intervals and Sample Size for Proportions**
- **Confidence Intervals for Variances and Standard Deviations**

## Module - 8: Hypothesis Testing
- **Traditional Method of Steps in Hypothesis Testing**
- **Z Test for a Mean and Proportion**
- **T Test for a Mean**
- **Chi-Square Test for a Variance or Standard Deviation**
- **Additional Topics Regarding Hypothesis Testing**

## Module - 9: Correlation and Regression
- **Scatter Plots and Correlation**
- **Regression**
- **Coefficient of Determination and Standard Error of Estimate (SEE)**
- **Multiple Regression**

## Module - 10: Analysis of Variance
- **One-Way Analysis of Variance**
- **The Scheffé Test and Tukey Test**
- **Two-Way Analysis of Variance**

---

## Demo Part: Applied Analysis with Statistics

- **Descriptive Statistical Analysis with Python**
- **Inferential Statistical Analysis with Python**
- **Real-Life Data Problem Solving with Python and Statistical Methods**


## Learning Style 
- **In Campus Class**
- **Online Live Class**
- **Online Recording (Google Classroom) Class**


## Class Fees 
- **In Campus ( 400,000 MMK ) per month**
- **Online Live Class ( 300,000 MMK ) per month**
- **Online Recording Class ( 400,000 MMK )**

### Contact
- **Phone - 09 2500 7400 8**
- **Viber - 09 2500 7400 8**
- *[Telegram](https://t.me/rom_dynamics)*
- *[Facebook ROM Robotics](https://www.facebook.com/ROMROBOTS/)*
- *[Facebook Deep Blue AI Lab](https://www.facebook.com/deepblueailab/)*

