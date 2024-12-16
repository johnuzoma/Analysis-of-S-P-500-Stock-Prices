### Executive summary
This is a project where I analysed S&P 500 stock prices. 
Techniques I used include (but not limited to): data ingestion, transformation, migration, subqueries, joins, aggregations, common table expressions, numeric and string functions.

### Business questions
My analysis provided answers to these questions:
1. Which date in the sample saw the largest overall trading volume?
2. On that date, which two stocks were traded most?
3. On which day of the week does volume tend to be highest?
4. On which day of the week does volume tend to be lowest?
5. On which date did Amazon (AMZN) see the most volatility, measured by the difference between the high and low price?
6. If you could go back in time and invest in one stock from 1/2/2014 - 12/29/2017, which would you choose?
7. What % gain would you realize?

### Data Pipeline
<img width="338" alt="image" src="https://github.com/user-attachments/assets/2728a69b-3b2d-42ad-8d72-464625f65ea2">

I ingested and transformed the data in MS Fabric using Dataflows and I migrated the data from Fabric to SQL Server using Copy activities.

### Analysis
The images of SQL code can be seen on the left-hand side. They are named "Q1.png" for Question 1, "Q2.png" for Question 2 etc.

The resultset is shown beneath the code in each image.

### Insights
1. The largest trading volume occurred on Feb 24, 2014. [Link to query](https://github.com/johnuzoma/Analysis-of-S-P-500-Stock-Prices/blob/main/Q1.png).
2. On that date, Verizon and Bank of America stocks were traded most with volumes of approximately 618 million and 103 million respectively. [Link to query](https://github.com/johnuzoma/Analysis-of-S-P-500-Stock-Prices/blob/main/Q2.png).
3. On average, Friday was the weekday with the highest volume. [Link to query](https://github.com/johnuzoma/Analysis-of-S-P-500-Stock-Prices/blob/main/Q3.png).
4. On average, Monday was the weekday with the lowest volume. [Link to query](https://github.com/johnuzoma/Analysis-of-S-P-500-Stock-Prices/blob/main/Q4.png).
5. The Amazon stock had the most volatility (~86) on June 9, 2017. [Link to query](https://github.com/johnuzoma/Analysis-of-S-P-500-Stock-Prices/blob/main/Q5.png).
6. If I could go back in time between Jan-02 2014 and Dec-29 2017, I would invest in Booking Holdings (PCLN) because it had the highest gain for the lowest volatility. [Link to query](https://github.com/johnuzoma/Analysis-of-S-P-500-Stock-Prices/blob/main/Q6.png).
7. I would have realised a 50% return on my investment if I had invested in Booking Holdings. [Link to query](https://github.com/johnuzoma/Analysis-of-S-P-500-Stock-Prices/blob/main/Q7.png).
