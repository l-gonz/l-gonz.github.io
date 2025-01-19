---
title: "Machine Learning emissions analysis"
subtitle: "Comparison of Energy Consumption in Machine Learning Models"
summary: "Comparing the energy usage of different machine learning algorithms to balance performance and sustainability."
tags: ["machine-learning", "python"]
complexity: "Intermediate"
date: 2022-04-20
github: "https://github.com/l-gonz/tfg-gitt-mlcost"
links:
  - icon: github
    icon_pack: fab
    name: Repository
    url: https://github.com/l-gonz/tfg-gitt-mlcost
---

## The MLCost application

Machine learning is powerful, but training large models consumes a lot of energy, impacting the environment. In this project, I developed a tool to measure and compare the energy usage of different machine learning algorithms. The goal was to help researchers balance model accuracy with energy efficiency.

The tool tracks carbon emissions using CodeCarbon and evaluates performance on public datasets. By understanding the trade-offs between accuracy and energy consumption, this project highlights the importance of sustainable AI development.

This application was developed as the Final Year project for my bachelor in Telecommunications Engineering. The project report is hosted in the [university's archive](https://hdl.handle.net/10115/38594) (in Spanish).

---

## Key Features
- **Energy Tracking**: Measures the carbon emissions of training machine learning models.
- **Performance Analysis**: Compares energy usage and accuracy for various algorithms like random forests, neural networks, and k-nearest neighbors.
- **Hardware Impact**: Assesses how resource configurations affect energy consumption using Microsoft Azure virtual machines to compare multiple machines.

---

## Tech Stack
- **Languages**: Python
- **Libraries**: scikit-learn (for Machine Learning), CodeCarbon (for emission calculation), Matplotlib (for graphs)
- **Platforms**: Microsoft Azure, Visual Studio Code

---

## How I Built It
### Design and Development
1. **Tool Architecture**: Built a modular application using scikit-learn for model training and CodeCarbon to monitor emissions.
2. **Experiments**: Conducted tests on open datasets of varying complexity, including Iris and EEG data.
3. **Visualization**: Used Matplotlib to create graphs comparing energy usage and accuracy.

### Key Results
- **Algorithm Comparison**: Neural networks offered high accuracy but had the highest energy consumption, while k-nearest neighbors consumed less energy with moderate accuracy.
- **Hardware Analysis**: Running models on more powerful machines increased energy use per second but reduced overall training time, balancing the total energy consumption.

---

## Software architecture
![Architecture of the application](images/gitt/arch.jpg)

---

## Results
![Emission scatter plot](images/gitt/scatter.png "Distributtion of emission and f-score values per model and dataset")
![Emission line graph](images/gitt/nsamples.png "Evolution of emission by ML model when increasing dataset sample size.")

Explore more:
- [GitHub Repository](https://github.com/l-gonz/tfg-gitt-mlcost)

---

## What’s Next?
I’d love to expand this project with:
- **More Models**: Including additional algorithms like transformers and CNNs.
- **Optimization**: Exploring ways to reduce energy consumption without sacrificing accuracy.

---

This project was a fascinating deep dive into the intersection of machine learning and sustainability, combining technical skills with environmental awareness.
