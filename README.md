# Lambda-Power-Tuning
How to determine Optimal LambdaMemory depending on Well Architected Pillar Priority
# AWS Lambda Performance & Cost Tuning

## Overview

This project explores how Lambda memory configuration affects
performance and cost.

Two complementary approaches were used:

1. AWS Lambda Power Tuning
   - Compared Lambda performance across different memory configurations
   - Evaluated execution time and cost

2. Postman Load Testing
   - Validated end-to-end API performance under simulated load
   - Measured throughput, latency, and errors

## Architecture

Postman
   |
   v
API Gateway
   |
   v
AWS Lambda
   |
   v
DynamoDB

## Experiment

The Lambda memory configuration was tuned using
AWS Lambda Power Tuning.

The selected configuration was then validated using
Postman performance testing.

## Postman Results

- Virtual Users: 10
- Duration: 2 minutes
- Total Requests: 2,682
- Throughput: 22.33 requests/sec
- Average Response Time: 320 ms
- P90: 361 ms
- P95: 396 ms
- P99: 594 ms
- Error Rate: 0%

## Key Learning

Lambda memory is not simply a memory setting.

Increasing memory also increases the compute capacity available
to the function, which can reduce execution time. The optimal
configuration therefore requires balancing:

Performance + Cost

Rather than choosing the largest memory configuration,
the goal is to find the point where additional compute
no longer provides enough performance benefit to justify
the additional cost.
