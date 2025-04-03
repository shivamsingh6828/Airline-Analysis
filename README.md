# ✈️ Airline Analysis Dashboard
# 📌 Overview
This Power BI dashboard provides a comprehensive airline performance analysis, tracking flight cancellations, delays, and on-time performance across multiple years.

# 📊 Key Metrics
- Total Flights Analyzed: 111K

- On-Time Flights: 79K

- Delayed Flights: 32K

- Cancelled Flights: 3K

- Average Delay Time: 19.0 minutes

# 📅 Flight Delay Insights
- Highest delays recorded in 2011 (49.72%)

- Delays distributed evenly across weekdays

- Flight delays consistently high on Fridays and Tuesdays

# 🛫 Flight Cancellation Trends
- Cancellation rates varied by airport (BWI, DCA, IAD)

- Highest cancellations recorded in 2010 (0.6K flights)

# 🛠️ Technologies Used
- Power BI for interactive visualizations

- DAX for advanced calculations

- Excel Data Sources – Airline records.

# 📌 DAX Measures Used
# 1️⃣ Total Number of Flights
  Total_Number_Flight = COUNT(Flights[Flight_ID])

 # 2️⃣ Total On-Time Flights
   Flight_On_Time = CALCULATE(COUNT(Flights[Flight_ID]), Flights[Status] = "On-Time")

  # 3️⃣ Total Flight Delays
   Flight_Delay = CALCULATE(COUNT(Flights[Flight_ID]), Flights[Status] = "Delayed")


