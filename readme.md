# (Flights Datasets  - Exploration)
## by (Alaa Alaboud)


### Flights Datasets

This dataset reports flights in the United States, including carriers, arrival and departure delays, and reasons for delays, from 1987 to 2008.

- we cleaned six years of flights datasets to use it in our investigate.
- our main datasets is `df_2008_clean`.
- We merged before these two data of flights years `1987.csv` and `1989.csv` after cleaning in this file `Flights_80.csv`. 
- We merged before these two data of flights years `1990.csv` and `1999.csv` after cleaning in this file `Flights_90.csv`.
- We merged before these two data of flights years `2000.csv` and `2008.csv` after cleaning in this file `Flights_20.csv`.
- we load the dataset `carriers.csv` that contains the full name for carriers code.
- we load the dataset `L_AIRPORT.csv_` that contains the full name for Airport for the origin IATA airport code, and the destination IATA airport code.

There are 700,977 flights in the United States in our dataset for the 2008 year after we make our Wrangling on it we keep the dataset with 23 features like LateAircraftDelay, UniqueCarrier, FlightNum, ArrDelay, Origin ... etc. 
The most variables are numeric in the dataset between integer and float, and the rest are a string object.



## Summary of Findings

- The most delay flights for the **2008** year is **21:56** hours. And the destination for that flight was from **Honolulu(HNL)** to **Los Angeles(LAX)** and the delay was in departure and arrival flight. The distance was **2556** miles, and the date for this flight was in **2008-07-30** on **wednesday**. Also the scheduled departure time local was at **14:45 pm**, but the actual departure time was at **12:41 pm**. And the scheduled arrival time was at **23:05 pm**, but the actual arrival time was at **21:10 pm**. The carrier was **American Airlines Inc.(AA)** and the flight FlightNum **(284)** and TailNum **(N392AA)**. The **National Air System(NAS)** got **9** minutes in delay, and we cant figure out the other reason for delay.
- The most reason to cancelation the flight is the **weather(B)**. And the less reason is the **security(D)** with just **12** canceled flights. And the second reason was the **carriers(A)** and it got **8%** from the database in cancellations type, likewise to the weather with the same percentage and difference in **574** canceled flights. And the  **National Air System(C)** reason got **4%** in our database that's a half percentage for weather and carriers reason.
- The **Southwest Airlines Co.(WN)** carrier recorded as the most carrier flights in **2008** at the United States with **1201754** flights, with the difference in **596869** flights with the second carrier **American Airlines Inc.(AA)**, and this is a huge difference. And the **Aloha Airlines Inc.(AQ)** carrier recorded as the fewer carrier flights with **7800** flights.
- The **American Eagle Airlines Inc.(MQ)** carrier recorded as the most carrier with cancelation flights in **2008** at the United States with **18331** flights, with the difference in **891** flights with the second carrier **American Airlines Inc.(AA)**. And the **Aloha Airlines Inc.(AQ)** carrier recorded as the fewer carrier with cancelation with **42** flights.
- In the waffle plot, we found  12% of the count of flights goes to Saturday, 14% for Sunday, 14% for Tuesday, 15% for Thursday, 15% for Friday, 15% for Monday and 15% for Wednesday. We can conclude from these that the flights' scheduled got full-time work in weekday and got part-time of work on a weekend day. 
- The best month with the most flights is **July(7)** with **627931** and the less is **November(11)** with **523272** flights. And there are 7 months recorded as the large month of flights with up than **60k** flights, the months are(**July-March-August-June-May**). And the rest months got between **59k** flights and **52k**.
- These days(**21, 14, 18, 7, 11, 3, 17, 10, 29, 2, 22, 15**) got **23k** flights, and the rest got **22k** flights. And the fewer days with flights is the (**31**), with **12k** flights, and that's because not all months have this day.
- In the **2008** year The preferred times for flight to occur was **6:00 AM** with **132059** flights and **7:00 AM** with **91952** flights with difference **40107** flight between them.
- In the **80s** The preferred time for the flight to occur was **7:00 AM** with **139778** flights with a large difference with the rest of times.
- In the **90s** The preferred time for the flight to occur was **7:00 AM** with **226501** flights with a large difference with the rest of times either.
- In the **20s** The preferred time for the flight to occur was **6:00 AM** with **187863** flights with a few difference with the **7:00 AM** that was got **181393** flights, and the difference just **6470** flights.
- The distribution of distance with arrival and departure delay seems to be alike. There are a big distribution on the short miles, but it goes less on longest miles. Also, there is a **positive correlation** between **distance** and **arrival delay**. And there is a **positive correlation** between **distance** and **departure delay**.
- There is **a monotonic** relationship between distance and the weekday. The distribution for **all days** is much peaked. And the **all days** seem as alike, from approximately **1200 miles** to **3700 miles** the distribution are much tinier from the **1000 miles** and down. The longtails suggest outliers on all days with the highest of distance miles from approximately **3700 miles** to over **5000 mails**. Finally, there isn't much different for the distribution on all days.
- The longest delay is in **Atlanta(ATL)** destination with approximately **360 minutes**, and with approximately **750** or **800 miles**. The second-longest delay is in **Chicago(ORD)** destination with approximately **240 minutes**, and with **800** or **850 miles**. Then also we have another long delay with **Chicago** and **Atlanta** destination, these destinations got the hight distance with a delay between **1** minute to **140 minutes**. The distribution for the delay with distance is got much distribution in the low distance then goes to less in the high distance. Finally, there is **a positive correlation** between **distance** and **late aircraft delay**.

## Key Insights for Presentation

### Insight(1)
The American Eagle Airlines Inc.(MQ) carrier recorded as the most carrier with cancelation flights in 2008 at the United States with 18331 flights, with the difference in 891 flights with the second carrier American Airlines Inc.(AA). And the Aloha Airlines Inc.(AQ) carrier recorded as the fewer carrier with cancelation with 42 flights.


### Insight(2)
In the 80s The preferred time for the flight to occur was at 7:00 AM with 139778 flights with a large difference with the rest of times. And In the 90s was at 7:00 AM with 226501 flights with a large difference with the rest of times either. Finally, In the 20s was at 6:00 AM with 187863 flights with a few difference with the 7:00 AM that was got 181393 flights, and the difference just 6470 flights.

### Insight(3)
The distribution of distance with arrival and departure delay seems to be alike. There are a big distribution on the short miles, but it goes less on longest miles. Also, there is a positive correlation between distance and arrival delay. And there is a positive correlation between distance and departure delay.

### Insight(4)
There is a monotonic relationship between distance and the weekday. The distribution for all days is much peaked. And the all days seem as alike, from approximately 1200 miles to 3700 miles the distribution are much tinier from the 1000 miles and down. The longtails suggest outliers on all days with the highest of distance miles from approximately 3700 miles to over 5000 mails. Finally, there isn't much different for the distribution on all days.

### Insight(5)
The longest delay is in Atlanta(ATL) destination with approximately 360 minutes, and with approximately 750 or 800 miles. The second-longest delay is in Chicago(ORD) destination with approximately 240 minutes, and with 800 or 850 miles. Then also we have another long delay with Chicago and Atlanta destination, these destinations got the hight distance with a delay between 1 minute to 140 minutes. The distribution for the delay with distance is got much distribution in the low distance then goes to less in the high distance. Finally, there is a positive correlation between distance and late aircraft delay.





