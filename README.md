# saas_user_analytics
####SaaS Analytics 
Data Intelligence & Business Insights Platform



Title Page 

SaaS analytics assignment 
Prepared by: Yashoratnam
Date: June 2025  
Organization: Project  


Objective : 
Design and implement an end-to-end data analysis pipeline using Python that helps a hypothetical SaaS business extract actionable insights from customer and product usage data. The intern will clean and transform raw data, perform advanced analytics (including cohort, retention, funnel, and churn analysis), visualize results, and deliver actionable insights to drive business strategy.

Scenario 
You are working with a SaaS platform that offers subscription-based access to productivity tools. The platform wants to understand customer behavior, product adoption, and growth metrics to inform decisions.
 

Data Collection 
Data provided by the sources is stored in separate CSV files via GitHub. 

Data Cleaning and Modelling 
Cleaned and transformed multiple raw datasets (users, subscriptions, events, support tickets) using pandas.
 All timestamp fields were standardized, and missing values, duplicates, and outliers were handled. 
Join all the cleaned datasets together and download that file for analysis. 
Writing extract, transform, and load functions to ensure the system.


Methodology
The analysis was carried out using a modular ETL pipeline and interactive visualizations, with Python and Plotly as the primary tools. The dataset consisted of user activity logs, subscription details, and support ticket histories. Performed EDA and anomaly detection to get business insights with recommendations. 


Data Analysis 
In this report, we analyze a subscription-based SaaS user dataset to understand growth patterns, engagement behaviors, and key performance metrics. The goal is to derive insights that guide product decisions, customer behavior, product adoption, and growth metrics.

User Growth by Signup Cohort (Month): Understand how user signups evolved and identify strong onboarding months. Cohort analysis also helped monitor retention behavior across join dates with enables us to know the product market in a specific period. The figure shows consistent growth over the months. 


Feature Adoption Patterns: Discover which subscription tiers utilize platform features most actively. Feature usage was analyzed by counting event_type (click, page) per plan.  Feature usage correlates — users’ interests in upgrades, justifying upsell efforts toward active Basic users.




Subscription Plan Trends (Churn, Upgrades, Downgrades): Track changes in plan subscriptions and evaluate churn behavior. Churn was defined by users whose subscription status was Cancelled. While Basic users have low churn, Pro and Enterprise users present the highest volatility, indicating friction in early-stage user experience.

Friction Points and Drop-Offs: Identify where users disengage or fail to convert.
 20% of users who signed up did not trigger any feature usage event. 
Key business metrics - 
Monthly Active Users (MAU) & Retention Rate: Track engagement month-by-month. Retention rate was derived by comparing users active in the current month vs. the previous. MAU grew steadily until June.
         Fast initial engagement correlates with lower churn, suggesting the need for in-app onboarding nudges and proactive support.

Revenue Analysis (ARR, MRR, ARPU): Understand revenue trends by geography and plan.
ARR (Annual Recurring Revenue) = active users × plan price × 12
MRR (Monthly Recurring Revenue) = active users × plan price
ARPU (Average Revenue Per User) = Total Revenue / Total Users
ARPU is highest in India and the UK due to more Enterprise and pro users. Region-specific upselling may enhance revenues.


                      SUBSCRIPTION STATUS




NPS Correlation (Satisfaction Score): Analyze whether user satisfaction influences retention or revenue. Where available, satisfaction_score was correlated with subscription duration and support resolution times. Users rating >8 had an average subscription period of 4.8 months vs. 2.1 months for those rating <6.

Faster resolution of support tickets and higher satisfaction scores are strong indicators of retention and upsell potential.

Funnel Analysis: Signup → Activation → Upgrade: Visualize the user journey and identify drop-offs. Signup: Users who created an account
Activation: Users who performed a feature-related event_type within 7 days
Upgrade: Users who moved from Trial or Basic to a paid plan. Most drop-off happens after the first feature use, indicating the need to deliver value earlier in the journey.




Insights
 User Growth by Signup Cohort: Consistent user growth indicates effective marketing and product-market alignment. Peak signup months enable us to have higher retention cohorts.
Feature Adoption Patterns:  Feature usage is significantly higher among Pro and Enterprise users. Basic-tier users show limited engagement with core features.
Subscription Plan Trends: Pro and Enterprise plans experience higher churn volatility despite being premium. Basic users exhibit stable usage but lower conversion to paid plans.
Friction Points and Drop-Off: 20% of users never triggered a single feature usage event post-signup. Most drop-offs occur before the user experiences value from the product. 
Monthly Active Users (MAU) & Retention Rate: MAU shows upward momentum; retention improves for users who engage early. Low engagement in the first week increases the likelihood of churn.
Revenue Metrics (ARR, MRR, ARPU):  ARPU is highest in India and the UK due to a strong Pro/Enterprise user base. MRR is stable but could grow with better conversion from trial to paid users.
 NPS and Satisfaction Correlation: Users with NPS >8 remain subscribed for 2x longer than detractors. Long support resolution times correlate with lower satisfaction and higher churn.
Funnel Analysis: Signup → Activation → Upgrade: Major drop-off happens after signup but before meaningful feature usage. Conversion from activation to paid upgrades remains modest.


Business Recommendations
 Analyze and double down on marketing strategies and onboarding practices from months with high signup or activation rates.
 Implement a guided onboarding checklist, showcase feature benefits in the first session, and introduce time-sensitive “first 5-day engagement” campaigns to reduce early churn.
 Monitor Day 1 and Day 7 user activities. Use inactivity as a trigger for personalized nudges via emails or SMS to drive activation.
 Introduce milestone rewards and gamified engagement journeys to sustain early user interest and encourage frequent feature use.
 Automate support responses, reduce ticket resolution time, and use NPS feedback loops to improve customer satisfaction and loyalty.
 Use usage thresholds to trigger personalized upgrade prompts, especially targeting engaged Basic users with in-app messages and Pro feature teasers.
 Create usage-based upgrade paths, offer loyalty rewards, and introduce concierge onboarding to convert Basic to Pro users.
Build machine learning models to identify and retain at-risk users. Combine with qualitative feedback surveys, especially from churned Pro users. 
 Identify high-ARPU geographies like India and the UK, and develop tailored pricing, bundles, and localized offers to boost revenue.
 Segment users by plan, region, and behavior. Personalize all messaging—whether for onboarding, upgrades, or re-engagement—to increase conversion and satisfaction.


References   
Python with commented commands: 
Saas analytics.ipynb

