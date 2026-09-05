# Lambda-Power-Tuning
How to determine Optimal LambdaMemory depending on Well Architected Pillar Priority
# AWS Lambda Performance Tuning

A beginner-friendly project demonstrating how to measure and optimize AWS Lambda performance using different memory configurations.

## 🎯 Objective

The goal of this project is to understand how AWS Lambda memory allocation affects:

* Execution time
* Performance
* Cost
* Overall application efficiency

The project uses a Lambda function that performs CRUD operations against Amazon DynamoDB.

## 🏗️ Architecture

```text
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
```

Lambda performance is then analyzed using AWS Lambda Power Tuning.

## ☁️ AWS Services Used

* AWS Lambda
* Amazon DynamoDB
* Amazon API Gateway
* AWS Step Functions
* AWS Lambda Power Tuning
* Amazon CloudWatch

## 🔧 Lambda Operations

The Lambda function supports the following operations:

| Operation | DynamoDB Action |
| --------- | --------------- |
| create    | PutItem         |
| read      | GetItem         |
| update    | UpdateItem      |
| delete    | DeleteItem      |
| list      | Scan            |
| echo      | Return payload  |
| ping      | Return pong     |

## 🧪 Performance Experiment

The same Lambda function is executed using different memory configurations.

Example:

```text
128 MB
256 MB
512 MB
1024 MB
1536 MB
```

For each configuration, we compare:

* Execution duration
* Cost
* Performance

The objective is to identify the configuration that provides the best cost/performance balance.

## 📊 Lambda Power Tuning

AWS Lambda Power Tuning is used to run the Lambda function with different memory configurations and visualize the results.

The experiment helps answer:

> What is the optimal Lambda memory configuration for this workload?

## 📈 Results

The performance results will be documented here after running the experiment.

|  Memory | Duration | Cost | Observation |
| ------: | -------: | ---: | ----------- |
|  128 MB |      TBD |  TBD | Baseline    |
|  256 MB |      TBD |  TBD | TBD         |
|  512 MB |      TBD |  TBD | TBD         |
| 1024 MB |      TBD |  TBD | TBD         |
| 1536 MB |      TBD |  TBD | TBD         |


## 📚 References

* AWS Lambda documentation
* AWS Lambda Power Tuning
* Amazon DynamoDB documentation
