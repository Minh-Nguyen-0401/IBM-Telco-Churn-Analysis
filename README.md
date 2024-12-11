# Telco Customer Churn Dataset

## Context
This sample dataset tracks a fictional telco company's customer churn based on a variety of possible factors. The `Churn` column indicates whether or not a customer left within the last month. Other columns include gender, dependents, monthly charges, and various details about the services each customer subscribes to.  
**Source:** IBM.

---

## Inventory of Telco Assets

### 1. Telco Churn
- **Description:** This sample dashboard tracks customer churn based on a variety of factors.
- **Key Data:** Includes `Churn Label` (whether the customer left within the last month), location, monthly charges, services, and customer lifetime value.
- **Location:** `Team content > Samples > Dashboards`.

### 2. Quarterly Churn Update
- **Description:** This sample story illustrates quarterly changes in customer churn, highlighting contracts and locations with the highest churn.
- **Key Data:** Includes `Churn Label` (whether the customer left within the last quarter).
- **Location:** `Team content > Samples > Stories`.

### 3. Customer Churn Information by Zip Code
- **Description:** Drill-through target report for the `Telco Churn` dashboard and `Quarterly Churn Update` story.
- **Location:** `Team content > Samples > Reports`.

### 4. Telco Churn Relationships
- **Description:** A sample exploration examining churn based on factors like location, monthly charges, and customer lifetime value.
- **Location:** `Team content > Samples > Explorations`.

### 5. Telco Customer Churn
- **Description:** This data module tracks churn based on factors such as gender, dependents, monthly charges, and services.
- **Location:** `Team content > Samples > Data`.
- **Source:** IBM.

#### Data Module Composition:
The `Telco Customer Churn` data module includes the following 5 uploaded files:
- `Telco_customer_churn_demographics.xlsx`
- `Telco_customer_churn_location.xlsx`
- `Telco_customer_churn_population.xlsx`
- `Telco_customer_churn_services.xlsx`
- `Telco_customer_churn_status.xlsx`

---

## Data Details

### Base Data
The `Telco Customer Churn` module contains 5 tables:
1. **Demographics**
2. **Location**
3. **Population**
4. **Services**
5. **Status**

Each table is described below:

---

### **1. Demographics**
- **CustomerID:** A unique ID that identifies each customer.
- **Count:** Used in reporting/dashboarding to sum up the number of customers in a filtered set.
- **Gender:** Male, Female.
- **Age:** Customer’s current age (in years) at the end of the fiscal quarter.
- **Senior Citizen:** Indicates if the customer is 65 or older (`Yes/No`).
- **Married:** Indicates if the customer is married (`Yes/No`).
- **Dependents:** Indicates if the customer has dependents (`Yes/No`).
- **Number of Dependents:** The number of dependents living with the customer.

---

### **2. Location**
- **CustomerID:** A unique ID that identifies each customer.
- **Count:** Used in reporting/dashboarding to sum up the number of customers in a filtered set.
- **Country:** The customer’s country of residence.
- **State:** The customer’s state of residence.
- **City:** The customer’s city of residence.
- **Zip Code:** The customer’s residential zip code.
- **Lat Long:** Combined latitude and longitude of the customer’s residence.
- **Latitude:** Latitude of the customer’s residence.
- **Longitude:** Longitude of the customer’s residence.

---

### **3. Population**
- **ID:** A unique identifier for each row.
- **Zip Code:** The customer’s residential zip code.
- **Population:** Estimated population for the zip code.

---

### **4. Services**
- **CustomerID:** A unique ID that identifies each customer.
- **Count:** Used in reporting/dashboarding to sum up the number of customers in a filtered set.
- **Quarter:** Fiscal quarter of the data (e.g., Q3).
- **Referred a Friend:** Whether the customer referred someone (`Yes/No`).
- **Number of Referrals:** The number of referrals made by the customer.
- **Tenure in Months:** Total months with the company by the end of the quarter.
- **Offer:** The last marketing offer accepted (`None`, `Offer A`, `Offer B`, `Offer C`, etc.).
- **Phone Service:** Subscribes to home phone service (`Yes/No`).
- **Avg Monthly Long Distance Charges:** Average long-distance charges up to the end of the quarter.
- **Multiple Lines:** Subscribes to multiple phone lines (`Yes/No`).
- **Internet Service:** Subscribes to internet service (`No`, `DSL`, `Fiber Optic`, `Cable`).
- **Avg Monthly GB Download:** Average monthly download volume in GB.
- **Online Security:** Subscribes to online security services (`Yes/No`).
- **Online Backup:** Subscribes to online backup services (`Yes/No`).
- **Device Protection Plan:** Subscribes to a device protection plan (`Yes/No`).
- **Premium Tech Support:** Subscribes to premium tech support (`Yes/No`).
- **Streaming TV:** Streams TV using the company’s internet service (`Yes/No`).
- **Streaming Movies:** Streams movies using the company’s internet service (`Yes/No`).
- **Streaming Music:** Streams music using the company’s internet service (`Yes/No`).
- **Unlimited Data:** Subscribes to unlimited data (`Yes/No`).
- **Contract:** Current contract type (`Month-to-Month`, `One Year`, `Two Year`).
- **Paperless Billing:** Chooses paperless billing (`Yes/No`).
- **Payment Method:** Payment method (`Bank Withdrawal`, `Credit Card`, `Mailed Check`).
- **Monthly Charge:** Total monthly charge for services.
- **Total Charges:** Total charges up to the end of the quarter.
- **Total Refunds:** Total refunds issued.
- **Total Extra Data Charges:** Total charges for extra data downloads.
- **Total Long Distance Charges:** Total long-distance charges.

---

### **5. Status**
- **CustomerID:** A unique ID that identifies each customer.
- **Count:** Used in reporting/dashboarding to sum up the number of customers in a filtered set.
- **Quarter:** Fiscal quarter of the data.
- **Satisfaction Score:** Overall satisfaction rating (1 = Very Unsatisfied, 5 = Very Satisfied).
- **Satisfaction Score Label:** Text version of the satisfaction score.
- **Customer Status:** Customer status at the end of the quarter (`Churned`, `Stayed`, `Joined`).
- **Churn Label:** Indicates if the customer churned this quarter (`Yes/No`).
- **Churn Value:** Binary indicator (`1` = churned, `0` = stayed).
- **Churn Score:** Predictive churn likelihood (0–100).
- **Churn Score Category:** Churn score grouped into ranges (e.g., 0-10, 11-20, etc.).
- **CLTV (Customer Lifetime Value):** Predicted lifetime value of the customer.
- **CLTV Category:** CLTV grouped into ranges (e.g., 2000–2500, 2501–3000, etc.).
- **Churn Category:** High-level reason for churn (`Attitude`, `Price`, etc.).
- **Churn Reason:** Specific reason for churn.

---

## Acknowledgements
This dataset is sourced from IBM. For more details, visit the original [IBM blog post](https://community.ibm.com/community/user/businessanalytics/blogs/steven-macko/2019/07/11/telco-customer-churn-1113).
```