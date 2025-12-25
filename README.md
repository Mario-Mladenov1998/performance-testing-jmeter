# Performance Testing with Apache JMeter

This project demonstrates basic performance testing using Apache JMeter
against the public API https://jsonplaceholder.typicode.com.

## Tools
- Apache JMeter 5.6.3
- Java 17

## Test Scenarios
- Smoke test with 1 user
- Load test with 50 users
- Load test with 100 users
- Load test with 200 users
- Load test with 500 users

## Test Details
- Endpoint: GET /posts
- Protocol: HTTPS
- Assertions: HTTP 200 OK
- Listeners: View Results Tree, Aggregate Report

## Results Summary (500 Users)
- Total requests: 500
- Error rate: 0%
- Average response time: ~165 ms
- 90% of requests under ~122 ms
- System remained stable under load

## Notes
Tests were executed for learning and portfolio purposes on a public demo API.


 Test Scenarios

The following test scenarios are included:
| Test Type                | Users | Description                                |
| ------------------------ | ----- | ------------------------------------------ |
| Smoke Test               | 1     | Basic availability and response validation |
| Load Test                | 50    | Moderate load validation                   |
| Load Test                | 100   | Increased concurrent users                 |
| Load Test                | 200   | High load scenario                         |
| Stress / Heavy Load Test | 500   | System behavior under heavy load           |


Metrics Observed

Response Time (Average, Min, Max)

Throughput (requests/sec)

Error Rate

Percentiles (90%, 95%, 99%)

All tests completed with 0% error rate.

/jmeter-tests
- jsonplaceholder_smoke_test_1_user.jmx
- jsonplaceholder_load_test_50_users.jmx
- jsonplaceholder_load_test_100_users.jmx
- jsonplaceholder_load_test_200_users.jmx
- jsonplaceholder_load_test_500_users.jmx

