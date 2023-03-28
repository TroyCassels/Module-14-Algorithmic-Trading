# Evaluation Report

## Overview

This file relates to an algorithmic trading bot for a top financial advisory firm.

Components of this analysis:

- Baseline analysis

- Tuning Baseline Trading Algorithm

- Evaluation of a New Machine Learning classifier

## Baseline Case

Training length: 3 Months

SMA values: short window = 4, long window = 100

<img width="575" alt="Screenshot 2023-03-28 at 1 19 59 pm" src="https://user-images.githubusercontent.com/119761709/228110406-6a2f5fc3-c28f-4879-b093-6efc600fc3fd.png">

For the baseline case, the strategy provides returns above actual returns i.e. it is a successful strategy.

## Tune algorithim - Adjust length of training dataset

Training length: 6 Months

SMA values: short window = 4, long window = 100

Increasing the training length significantly improved performance of the strategy.

<img width="575" alt="Screenshot 2023-03-28 at 1 29 57 pm" src="https://user-images.githubusercontent.com/119761709/228111844-b2841b5e-2c0a-48d9-ae22-57771cac10fb.png">

## Tune algorithim - Adjust length of SMAs

Training length: 3 Months

SMA values: short window = 10, long window = 150

Changing the length of the SMAs made performance worse.

<img width="575" alt="Screenshot 2023-03-28 at 1 32 51 pm" src="https://user-images.githubusercontent.com/119761709/228112380-1f219266-9638-4397-ba08-2da034c34e21.png">

## Conclusion for SVM

Adjusting the length of the training window from 3 to 6 months provides the biggest increase in the strategy.

<img width="575" alt="Screenshot 2023-03-28 at 1 29 57 pm" src="https://user-images.githubusercontent.com/119761709/228113081-bdc2abec-db9c-4fe9-a2af-2aca6d49aa5f.png">

## Alternative model - Adaboost

This model did not perform as well as the tuned model.

<img width="575" alt="Screenshot 2023-03-28 at 1 42 06 pm" src="https://user-images.githubusercontent.com/119761709/228113590-93512c93-aa76-414b-8ec4-696e67f114ad.png">



