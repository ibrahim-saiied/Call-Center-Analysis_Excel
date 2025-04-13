# Call Center Analysis - Excel

### Link to [Interactive Dashboard on novyPro](https://www.novypro.com/profile_about/ibrahim-saiied-1?Popup=memberProject&Data=1744451745063x789127784113938900) 
### Link to [MY Linked In](https://www.linkedin.com/in/ibrahim-saiied-data-analyst/) 
<br>
<div align="center">
    <img src="https://github.com/user-attachments/assets/be630b01-a423-4a63-b310-c4e74190e1db" alt="image" width="1000" height="500">
</div>


## Introduction
<details>
   <summary><strong>📌 Overview (click)</strong></summary>

 ### **Overview**  
> This Excel Analysis project provides a detailed analysis of **NBE Bank Call center** performance, covering **KPIs Performance**, **Call's Volume**, and **Customers needs**.  
> The analysis aims to uncover insights to improve customer service performance, such as reducing hold time by 10.8% and increasing 5-star ratings from 61.6%. It also prioritizes areas for improvement, such as Tech Support's low 8% resolution rate.

</details>


<details>
   <summary><strong>📂 Data Sources (click)</strong></summary>

### **Data Sources**  
> The primary dataset used for this analysis is the **"Fact_Call_Center"** Sheet containing detailed information about each Call.  

**▼ 📑Dataset Files Explanation** [[Download]](https://raw.githubusercontent.com/ibrahim-saiied/Call_center/refs/heads/main/Data%20Set/Call%20Center%20(Dataset).rar)  


1. **Fact_Call_Center Sheet**  
   > - **<ins>Call ID</ins>**: Unique **ID** for each **Call**. 
   > - **<ins>Agent</ins>**: Unique ID for each **Agent** working on the call.
   > - **<ins>Date</ins>**: Date of receiving the call.
   > - **<ins>Time</ins>**: Time of receiving the call.
   > - **<ins>Topic</ins>**: Topic discussed on the call. Foreign Key for **Dim_Topic table**.
   > - **<ins>Call Type</ins>**: Inbound or Outbound. Foreign Key for **Dim_CallType table**.
   > - **<ins>Answered</ins>**: Indicates whether the call was answered or not.
   > - **<ins>Resolved</ins>**:: Indicates whether the issue was resolved during the call.
   > - **<ins>Abandoned</ins>**:: Indicates whether the caller abandoned the call before being attended.
   > - **<ins>AnsweringTime</ins>**:: Time taken for an agent to answer the call after it enters the queue (from ringing to pickup).
   > - **<ins>WaitTime</ins>**:: Total time the caller spent waiting in queue (includes IVR time, excludes ringing).
   > - **<ins>AvgTalkDuration</ins>**:: Average duration of the conversation between agent and caller (excluding hold time).
   > - **<ins>AvgHoldDuration</ins>**:: Average time the caller was put on hold during the call (may include multiple hold events).
   > - **<ins>AfterCallWork</ins>**:: Time agent spent on post-call activities before becoming available for the next call.
   > - **<ins>SatisfactionRating</ins>**:: Customer Satisfaction Score (CSAT), typically rated 1–5.
   > - **<ins>QAScore</ins>**:: Internal Quality Assessment score based on criteria like script adherence and professionalism.
   > - **<ins>FirstCall</ins>**:: Indicates if the issue was resolved during the first call (used to track First Call Resolution).
   > - **<ins>FlaggedCall</ins>**:: Indicates if the call was flagged for review due to complaints, unusual behavior, or policy concerns.
   > - **<ins>Escalated</ins>**:: Indicates if the call was escalated to a higher-level agent or supervisor.

2. **Dim_Agent Sheet**  
   > - **<ins>Agent ID</ins>**: Unique ID for each **Agent**.  
   > - **<ins>First Name</ins>**: First Name of each **Agent**.
   > - **<ins>Last Name</ins>**: Last Name of each **Agent**. 
   > - **<ins>Ethnicity</ins>**: The self-reported ethnicity of the agent, used for diversity and inclusion reporting.
   > - **<ins>Gender</ins>**: The gender of the agent (e.g., Male, Female).
   > - **<ins>Team</ins>**: The team or department the agent belongs to.

3. **Dim_Topic Sheet**
   > - **<ins>CallType ID</ins>**: A unique identifier for the type of call. Used as a primary key to link with fact tables.
   > - **<ins>CallType</ins>**: The category of the call (e.g., Inbound, Outbound).

</details>

<!-- ------------------------------------------------------------------------------------------- -->

## Case Study
NBE call center supports many customers across different regions and receives a high number of calls every day. lately, the company has received complaints about long waiting times and poor service, some customers have even stopped using the service because of these issues.

Before growing the business further, the management team asked for an Excel dashboard to track important performance indicators like Answer Rate, Service Level, First Call Resolution (FCR), Customer Satisfaction (CSAT), and peak call times.
The main goal is to understand where the problems are, improve team scheduling, and provide better service using clear and simple data.

## Main 𝐊𝐏𝐈𝐬
- **<ins>Service Level (%)</ins>**: (Target: > 91.5%) Percentage of calls answered within your target time (30s).
- **<ins>Answer Rate (%)</ins>**: (Target: > 95%) Percentage of calls answered vs. total calls received.
- **<ins>Hold Time (%)</ins>**: (Target: < 10%) Percentage of time callers wait on hold from total in the call after answering. 
- **<ins>First Call Resolution (FCR %)</ins>**: (Target: > 80%) Percentage of problems solved in the first call.
- **<ins>Customer Satisfaction (CSAT %)</ins>**: (Target: > 4.4) Rating of Satisfaction customers (rated 1-5 stars).
- **<ins>Average Handle Time (AHT)</ins>**: (Target: < 10:30) Average time agents spend per call without waiting time.

## Process
1) Explored and validated the call center data
2) Imported and cleaned data using Power Query with helper columns
3) Built a data model
4) Created key measures using DAX (e.g., SL, FCR, CSAT)
5) Designed an interactive Excel dashboard to visualize insights

## Measures





















