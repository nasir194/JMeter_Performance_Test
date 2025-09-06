## Summery -
  - Here I have performed Load Test and Stress Test on Booking APIs.

## Test scenarios -
1. Create a Collectio of APIs (JMeter Collection) of Login API, Create Booking API and Search API Http requests.
2. Perform Load Test and Stress Test. Find the Bottleneck point and Capacity Point.
- Website for APIs - https://restful-booker.herokuapp.com

Scenario: 120,000 users over a 12-hour period log in, create a booking, and search for the booking.

- Todo 1: Find the throughput and perform a load test to a maximum of 20 minutes to save time to ensure the server can handle the load. Create a load test report. Use a Gaussian Random Timer (Deviation 2000ms, Constant delay 500ms). Do it in 3 step 1st step: 5 min load 2nd step: 10 min load 3rd step: 20 min load
- Todo 2: If the load test passes, identify the bottleneck throughput by conducting a stress test. Create a stress test report. 
- Todo 3: Generate an HTML report for both the load test and the stress test.

## How to run?
### Execute the following steps using JMeter:
- ``` git clone https://github.com/nasir194/JMeter_Performance_Test ```
- ``` Open ApacheJMeter ```
- ``` From ApacheJMeter open the JMX File and Run ```

### Execute the following steps using CLI:
- ``` git clone <repo_url> ```
- ``` jmeter -n -t .\Booking.jmx -l .\Booking.jtl -e -o Reports ```

### Generated HTML report for Load Test -
<img width="1098" height="585" alt="load test" src="https://github.com/user-attachments/assets/0e7b1f61-8895-4b3f-98eb-b4ad26d60948" />


### Generated HTML report for Stress Test -
<img width="1105" height="595" alt="stress test" src="https://github.com/user-attachments/assets/ad253ec7-8c7e-4204-abf1-fb8850d9f710" />



