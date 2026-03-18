
#**AI-Powered Parametric Income Protection for Food Delivery Workers.**

##**Problem Statement**

Gig economy workers such as food delivery partners depend completely on daily earnings. Platforms like Swiggy and Zomato employ thousands of delivery workers who rely on consistent order flow to earn income.
However, external disruptions such as:
-	heavy rainfall
-	extreme heat
-	severe pollution
-	platform outages
-	city restrictions
can significantly reduce delivery orders.
During such events, delivery partners experience income loss despite being willing to work.
Traditional insurance products do not address temporary income disruption.
Therefore, this project proposes an AI-powered parametric insurance platform that automatically compensates delivery workers when predefined disruption conditions occur.
The goal is to provide financial stability and risk protection for gig workers.


##**Persona**

-    Name: Ramesh Kumar
-    Age: 27
-    Platform: Swiggy
-    City: Hyderabad
-    Vehicle: Motorcycle
-    Average Daily Orders: 18
-    Average Daily Income: ₹700 – ₹900
-    Working Hours: 10 hours/day

Challenges faced:

1.	Extreme Weather
-	Heavy rain reduces customer orders.
-	Heatwaves make working dangerous.
2.	Platform Downtime
-	If the delivery app crashes, he cannot accept orders.
3.	Environmental Conditions
-	Severe pollution affects rider safety.
These disruptions cause immediate loss of daily earnings.


##**Proposed Solution**

The proposed solution is an AI-driven parametric insurance platform designed specifically for food delivery workers.
Workers subscribe to a weekly micro-insurance plan that protects their income from disruptions.
The system continuously monitors external data sources such as:
-	weather APIs
-	pollution APIs
-	platform availability
If a predefined condition is triggered, the system automatically initiates a claim and payout without requiring the worker to submit a request.
This ensures:
-	quick compensation
-	minimal paperwork
-	transparent claims process

##**Weekly Premium Model**

The platform offers weekly subscription-based coverage.

Plan
| Plan | Weekly Premium | Maximum Payout |
|------|---------------|----------------|
| Basic | ₹20 | ₹500 |
| Standard | ₹40 | ₹1000 |
| Premium | ₹60 | ₹1500 |

Workers can choose a plan depending on their daily income level.



##**Parametric Triggers**

For food delivery workers, the following are the conditions where the worker may not be able to work.
1.	Extreme Heat
Condition:
    Temperature > 45°C
Impact:
    Delivery riders cannot safely work in extreme heat.
2.	Heavy Rainfall
Condition:
    Rainfall > 80 mm
Impact:
    Customers cancel orders and riders cannot travel easily.
3.	Severe Air Pollution
Condition:
    AQI > 400
Impact:
    Working outdoors becomes hazardous.
4.	Platform Outage
Condition:
    Food delivery platform downtime > 30 minutes
Impact:
    Workers cannot receive delivery requests.


##**Application Workflow**

Step 1: Worker Registration
Information collected:
-	name
-	delivery platform
-	city
-	average income
-	preferred insurance plan
Step 2: Policy Purchase
-	Worker selects a weekly plan and activates coverage.
Step 3: Risk Monitoring
The system continuously monitors:
-	weather data
-	pollution levels
-	platform availability
Step 4: Event Detection
If a disruption occurs, the system checks whether it meets the parametric trigger conditions.
Step 5: Claim Validation
System verifies:
-	worker location
-	active policy
-	eligibility
Step 6: Automatic Claim Creation


Step 7: Instant Payout
Compensation is transferred through digital payment methods such as:
-	UPI
-	bank transfer
-	digital wallet

##**AI / ML Integration**

1.	Risk Prediction Model
We need a Risk Prediction Model to estimate how likely delivery disruptions are in a city for a particular week.
Our model will use:
-	Temperature data 
-	Rainfall data 
-	Air Quality Index (AQI) 
-	Historical disruption data
-	Location 
Output of the model
The model produces a Risk Score.

2.	Dynamic Premium Adjustment
This is used to ensure fair pricing of insurance plans based on risk levels.
Based on this risk score, the weekly premium for each insurance plan may be adjusted slightly.
Higher disruption probability results in slightly higher premiums, while lower risk periods maintain standard pricing.
However, the coverage amount associated with each plan remains fixed, ensuring transparency for delivery workers.
Each policy remains active for a period of 7 days from the time of purchase.
At the end of the coverage period, the worker can renew the policy by paying the premium again, ensuring continued protection against income disruptions.
If the worker chooses not to renew the policy, the coverage simply expires without any penalty.
Later, again if the worker decides to pay the insurance, he can continue the same policy.

3.	Fraud Detection
Your system gives automatic payouts when disruptions occur.
Some workers might try to cheat the system to get money even when they are not eligible.
Fraud detection ensures only genuine workers receive payouts.
The system checks:
-	Worker GPS location
-	Event location (rain / heat zone)
-	Policy active status
-	Worker activity on delivery platform
-	Previous claims
If fraud is detected then payout is blocked.



##**Technology Stack**

Frontend
React.js
Features:
-	worker registration
-	policy selection
-	dashboard
-	claim notifications
Backend
Spring Boot
Services:
-	user management
-	policy management
-	claim automation
-	event detection
AI Layer
Python
Libraries used:
-	scikit-learn
-	pandas
-	numpy
Database
PostgreSQL
Tables include:
-	users
-	policies
-	events
-	claims
-	payments
System Architecture
Frontend (React Web App)
       ↓
Backend API (Spring Boot)
       ↓
Event Monitoring Service
       ↓
AI Risk Engine (Python)
       ↓
Policy & Claim Management System
       ↓
Payment Gateway
       ↓
Database



##**Development Plan**

Phase 1
-	research
-	idea development
-	architecture design
-	documentation
Phase 2
-	prototype development
-	API integration
-	AI model implementation
Phase 3
-	testing
-	user interface improvements
-	demo preparation


##**Expected Impact**

The proposed system will:
-	provide financial protection for gig workers
-	reduce economic uncertainty
-	automate insurance claims
-	promote digital insurance adoption
This solution has the potential to improve financial resilience for millions of delivery workers.


