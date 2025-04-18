### Example: Chain-of-Thought Prompt

**Prompt:**
You are an AI assistant. When solving problems, think step-by-step to ensure accuracy. For example:

**Sources:**
[Yahoo ](https://finance.yahoo.com/)
https://www.google.com/finance/?hl=en


**Question:** For each traded investment in the Investment_of_interest collect the following most current values the dividend yield, the ex-dividend date, the next quarterly earnings report, the investment type, and the market?

**Output Type:** Create the output as a table with 6 columns and one row for each of the investments listed in the Investment_type.

**Definitions:**
1. Investment_type=(Equity-US, ETF-US, Equity-dividend, ETF-dividend, PreciousMetal)
2. Market_type=(Small_biotech, US_SP500, International_large)
3. Investment_of_interest=(AMZN,BYDDY,IVV)

**Step-by-Step Reasoning:**
1. Select the investment ticker from the Investment_of_interest list. For example the first stock on the list is AMZN.
2. Pull today's date.
3. Using (google finance or yahoo finance), today's date and the ticker find the current dividend yield. If there is no dividend yield leave the field blank.
4. Using (google finance or yahoo finance), today's date and the ticker find the next date for the ex-dividend date. If there is no ex-dividend date leave the field blank.
5. Using (google finance or yahoo finance), today's date and the ticker find the next date for the ex-dividend date. If there is no ex-dividend date leave the field blank.
6. Using (google finance or yahoo finance) to select the best catagorical Investment_type for the stock of interest.


The train's speed is 60 miles per hour.
2. The train travels for 2 hours.
3. To find the distance, multiply speed by time: 60 miles/hour × 2 hours = 120 miles.
4. Therefore, the train travels 120 miles.

**Answer:** 120 miles.

Now, use this step-by-step reasoning to solve the following question:
Create a table with 4 columns: 
