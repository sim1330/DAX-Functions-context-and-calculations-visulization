# DAX-Functions-context-and-calculations-visulization

Project Goal
The primary goal of this mini-project is to demonstrate proficiency in DAX (Data Analysis Expressions) by implementing various functions and mastering Evaluation Contexts (Row Context and Filter Context) within a Power BI or tabular data model.

Suggested Project Titles
DAX Context Deep Dive: Sales & Inventory Analysis

Mastering Filter Context: A DAX Mini-Project

DAX Calculations Showcase

That's a fantastic idea. Writing the project documentation in your own voice makes it more authentic and impactful.

Here is a draft for your README.md file, written from your perspective, emphasizing your DAX expertise and the project's structure.

🎯 DAX Mastery Mini-Project: Unpacking Evaluation Contexts
Hello! Welcome to my mini-project, where I dive deep into the world of DAX (Data Analysis Expressions) within Power BI. This project isn't just about creating metrics; it's about demonstrating my strong understanding of Evaluation Contexts—the single most critical concept for writing robust and accurate DAX.

My goal here was to create a set of insightful, functional measures by intentionally manipulating Filter Context and forcing Context Transition to prove proficiency beyond simple aggregation.

🛠️ Project Structure and Technology
Technology: Power BI Desktop (for data modeling, DAX calculations, and visualization)

Data Source: (Insert Your Data Source, e.g., A cleaned mock sales dataset)

Project File: DAX_Mini_Project.pbix

Code Reference: DAX_Measures_Script.txt (All major measures documented for quick review)

🔑 Core DAX Concepts Demonstrated
I focused on implementing advanced scenarios to showcase control over the DAX engine:

1. Filter Context Manipulation with CALCULATE
I used the powerful CALCULATE function not just for simple filtering, but to completely override the incoming Filter Context.

Demonstration: Creating Time Intelligence metrics (like Year-over-Year change) and comparison metrics (like Sales vs. All Regions) using functions such as SAMEPERIODLASTYEAR, DATEADD, and filter modifiers like ALL and ALLEXCEPT.

2. Context Transition
This is the critical step. I explicitly created Calculated Columns and then used an embedded CALCULATE function within an Iterator (SUMX or AVERAGEX) to force the Row Context to transition into a new Filter Context.

Demonstration: Calculating the Sales-to-Average-Price ratio per row, where the 'Average Price' needs to be calculated across the entire filter set, not just the single row.

3. Iterators (X functions)
I leveraged Iterators (like SUMX and AVERAGEX) to perform row-by-row calculations before aggregation, which is essential for accurate margin and weighting calculations.
