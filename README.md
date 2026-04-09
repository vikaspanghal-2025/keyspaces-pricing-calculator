# Amazon Keyspaces Pricing Calculator 🚀

Interactive pricing calculator for Amazon Keyspaces (for Apache Cassandra) that helps estimate costs based on read/write throughput, storage, and capacity modes.

**[Try the Calculator](https://aws-samples.github.io/sample-pricing-calculator-for-keyspaces/)**

**Source:** [aws-samples/sample-pricing-calculator-for-keyspaces](https://github.com/aws-samples/sample-pricing-calculator-for-keyspaces)

## What It Does

Provides a quick, interactive way to estimate monthly Amazon Keyspaces costs without needing to manually calculate pricing from the AWS pricing page. Input your workload parameters and instantly see cost breakdowns for both Provisioned and On-Demand capacity modes.

## Features

- **Dynamic Cost Estimation** — Calculate approximate monthly charges based on read/write throughput, average row size, storage needs, TTL deletes, and more
- **Multi-Region Support** — Optionally replicate to up to five AWS Regions and see how replication affects total cost
- **Provisioned vs. On-Demand** — Compare both capacity modes side-by-side to determine the best pricing strategy for your use case
- **Point-in-Time Recovery (PITR) Toggle** — Include or exclude PITR in your cost estimates

## Configuration Parameters

| Parameter | Description |
|-----------|-------------|
| Primary AWS Region | Where your Keyspaces data primarily resides (e.g., us-east-1) |
| Replicate to AWS Regions | 0-5 optional regions for multi-region replication |
| Average Read Requests | Estimated read requests per second (per region) |
| Average Write Requests | Estimated write requests per second (all regions) |
| Average Row Size (Bytes) | Size of each row in bytes (e.g., 1024 for 1 KB) |
| Storage (GB) | Total data stored in gigabytes |
| Point in Time Recovery | Enable/disable PITR to see cost impact |
| TTL Deletes per Second | Estimated TTL-based row deletions per second |

## Getting Started

Visit the [live calculator](https://aws-samples.github.io/sample-pricing-calculator-for-keyspaces/) or clone the [source repository](https://github.com/aws-samples/sample-pricing-calculator-for-keyspaces) to run locally.

## Disclaimer

This calculator is an estimation tool only. Actual AWS costs will vary based on factors like data distribution, network usage, and additional services. Always consult the official [Amazon Keyspaces pricing](https://aws.amazon.com/keyspaces/pricing/) for the most up-to-date information.

## License

MIT-0 License — see the [source repository](https://github.com/aws-samples/sample-pricing-calculator-for-keyspaces) for details.
