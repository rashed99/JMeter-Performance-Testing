# Restful-Booker API Performance Testing

## Project Summary: 
I performed Load Testing and Stress Testing on the Restful Booker API using Apache JMeter. The testing covered three APIs: Login, Create Booking, and Search Booking.
The business requirement was to handle 120,000 users over 12 hours. Based on this requirement, I calculated the target throughput and performed Load Testing in three stages: 5, 10, and 20 minutes. After Load Testing, I performed Stress Testing by gradually increasing the load and stopped the test when the error rate approached 1%.

## Technology:
- Apache JMeter
- JMeter CLI
- JMeter Dashboard Report

## Prerequisite:
- Java JDK 8+
- Apache JMeter

## How to run?
- Download the booking.jmx file from this repository.
- Open a terminal in the folder containing booking.jmx
- Run Load Test:
jmeter -n -t booking.jmx -l load-results.jtl -e -o load-report
- Run Stress Test:
Increase the Number of Threads in JMeter, save the test plan, and run:
jmeter -n -t booking.jmx -l stress-results.jtl -e -o stress-report
- Open index.html inside the generated report folder to view the results.

##  Load Test Report
<img width="754" height="285" alt="image" src="https://github.com/user-attachments/assets/3db16c4d-35db-4e88-b411-9a38911dc48e" />

##  Stress Test Report
<img width="752" height="280" alt="image" src="https://github.com/user-attachments/assets/cf9ef5bc-b7de-4673-b28c-3e9146edfbc0" />



