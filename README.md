# Power BI Project: Call Center Performance Analysis

This Power BI project analyzes call center data to provide insights into key performance indicators (KPIs) and agent performance.

## Project Overview

*   **Purpose:** This project aims to analyze call center data to understand call patterns, agent performance, and overall call resolution effectiveness. The goal is to create an interactive report that provides actionable insights for management.

## Data Source(s)

*   The data for this project comes from a call center dataset containing the following columns:
    *   `CALLER ID` (Unique identification number of each caller)
    *   `AGENT` (Name of the agent who handled the call)
    *   `DATE` (Date when the call was received)
    *   `TIME` (Time the call was received in hh:mm:ss format)
    *   `TOPIC` (Subject of the call)
    *   `ANSWERED` (Indicates if the call was answered - "Y" or "N")
    *   `RESOLVED` (Indicates if the call was resolved - "Y" or "N")
    *   `SPEED OF ANSWER IN SECOND` (Speed at which the call was answered)
    *   `AVG. TALK DURATION` (Average duration of the call)
    *   `SATISFATION RATE` (Satisfaction rating provided by the caller)
* The data source is in an unspecified file, if it is in the repo mention it e.g.,"The raw data is located in the `call_center_data.csv` file".

## Data Preparation

The following steps were performed to prepare the data for analysis:

*   **Null Value Handling:** All null or blank values were replaced with 0.
*   **Data Type Conversion:** Data types were adjusted where needed to ensure accurate analysis (e.g., converting date/time columns to date/time types, numerical columns to numeric types).
*   **Duration Calculation:** The `AVG. TALK DURATION` column was used to extract seconds and minutes. A new column, named `Duration on calls` (datatype changed to number in seconds), was created to represent the total duration of the call in seconds.

## Report Design

The interactive report includes the following KPIs and analyses:

*   **Total Number of Calls:** Calculated the total number of calls received.
*   **Answered vs. Rejected Calls:**
    *   A new column was created to calculate total number of calls answered and total number of calls been rejected.
    *   The percentage of calls answered and rejected were calculated and displayed.
*   **Resolved vs. Not-Resolved Calls:**
    *   New columns were created to calculate the number of calls resolved and the number of calls not resolved.
*   **Top Performing Agents:**
    *   Identified the top 1 agent who answered the maximum number of calls.
    *   Identified the top 1 agent who achieved the highest satisfaction rate.
*   **Call Volume by Topic:** A chart (e.g., bar chart) is used to visualize total calls by topic.
*   **Call Duration by Agent:** Visualizes the total duration of calls by each agent.
*   **Call Trends:**
    *   Total number of calls were aggregated by days and months for the year 2021.
    *   Slicers are included to filter charts by month and day for interactivity.
*   **Overall Performance:** The report includes overall 2021 performance rating
* **Overall Satisfaction Rating**: The report uses a custom visual to show the satisfaction rating.
* **Visualizations:** The report uses multiple types of visuals for representation and understanding of the data such as: **Pie Charts**, **Cards**, **Bar Charts** and **Slicers**

## Key Learnings

*   Through this project, I gained a better understanding of call center operations, particularly how customer satisfaction is measured and tracked.

## Usage

*   This report is designed to be used by call center managers and team leaders to monitor performance, identify trends, and optimize agent performance.
