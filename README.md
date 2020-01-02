# Introduction
For insurance companies it is of financial relevance to detect fraudulent claims as early as possible to be able to react accordingly (e.g. reject the claim). A common approach is often a simple fact check (e.g. if the historic weather data allow a weather-related claim), which is often executed by a claim adjuster. This can also be (partly) automatized by extracting information out of the claim-description document and other available data sources. However, chances are high that an automatized stand-alone fact check identifies a very limited number of potential fraud-cases.
Moreover, insurance companies have historical knowledge of fraud cases in the past and it makes sense to use this common memory. This Use Case describes how data science techniques can be used to archive a better detection rate based on historic data. The idea is to train an artificial neural network (ANN) on the company's past data and use it after the learning process to identify new potential fraud cases.

# Data Setup
## Prerequisites
Every data base will have different data items which can be used in setting up an ANN. But a field indicating if a historic claim-record has been identified to be fraud is mandatory. This yes/no field is essential for training the ANN and the boolean variable is also the outcome of the model.

# Design of ANN
TODO

# Outcome
The quality of Fraud modelling can be determined by looking at certain indicators, like the accuracy rate. Basically, two error types can occur, which are familiar from hypothesis testing:
- Type 1 Error (false positive): a non-fraud claim is classified as fraud
- Type 2 Error (false negative): a fraud claim is not classified as fraud
