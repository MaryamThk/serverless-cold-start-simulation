# serverless-cold-start-simulation
A Python simulation project comparing simple policies for reducing cold start latency in serverless systems.


This repository contains a course project for an Advanced Operating Systems course.  
The project studies the impact of cold start latency on response time in serverless systems.

## Project Idea

In serverless computing, functions are executed only when needed. If a function is not already prepared, the platform must initialize its execution environment before serving the request. This initial delay is known as a cold start.

The goal of this project is to simulate cold start behavior and compare three simple policies:

1. On-demand execution
2. Always-warm execution
3. Smart warming for frequently used functions

## Simulation Setup

The simulation was implemented in Python and uses 1,000 randomly generated requests.

Five sample functions were considered:

- login
- search
- payment
- upload
- report

For each function, the simulation defines a normal warm response time and an additional cold start delay.

## Evaluation Metrics

The policies were compared using four metrics:

- Average response time
- Maximum response time
- Number of cold starts
- Average resource usage

## Main Result

The always-warm policy achieved the lowest response time and eliminated cold starts, but it consumed the most resources.

The smart-warming policy reduced the number of cold starts and improved average response time compared with the on-demand policy, while increasing resource usage only slightly.

Therefore, smart warming provides a better balance between performance and resource usage.

## Tools

- Python
- Google Colab
- NumPy
- Pandas
- Matplotlib

## Author

Maryam Tehranikia
