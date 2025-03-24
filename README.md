# Ship Fire Simulations and Bot Strategies

<div align="center">
  <img src="https://github.com/user-attachments/assets/d33450be-f031-4e11-bd48-0ab0e0c3dadb" alt="Simulation Snapshot" style="height: 300px; border: 2px solid #000; margin: 20px auto;" />
</div>

This repository contains a comprehensive suite of projects developed as part of the Intro to Artificial Intelligence (CS 520) course at Rutgers University. The projects simulate a realistic spaceship environment to evaluate various bot strategies under dynamic, hazardous conditions. The work integrates simulation techniques, probabilistic modeling, advanced pathfinding algorithms, and deep learning to address complex navigation and target localization challenges.

## Overview

### Ship Fire Simulation & Bot Strategies
- **Simulation Environment:**  
  - Created a 40×40 grid-based model of a spaceship with randomly distributed obstacles and dynamic fire sources.  
  - Incorporated a fire spread mechanism with adjustable flammability parameters to simulate unpredictable, hazardous conditions.
  
- **Bot Strategy Implementation:**  
  - Designed and compared four distinct bot strategies:  
    1. **Static BFS Bot:** Computes a single optimal path without accounting for fire dynamics.  
    2. **Adaptive BFS Bot:** Recalculates the shortest path at every step to avoid active fire zones.  
    3. **Enhanced BFS Bot:** Extends the adaptive approach by also avoiding cells adjacent to fires.  
    4. **Adaptive A* Bot:** Utilizes an A* algorithm with a custom heuristic that balances distance and fire risk.
  
- **Performance Evaluation:**  
  - Conducted 10 fire spread scenarios with 100 trials each.  
  - Achieved up to a 40% reduction in failure rates using adaptive strategies versus static pathfinding.

### Space Rats – Probabilistic Localization & Pathfinding
- **Sensor-Based Localization:**  
  - Engineered a sensor-driven 30×30 grid model to generate probability distributions for the target ("space rat") location.  
  - Implemented digital signatures for each open cell to uniquely identify and track potential target positions.
  
- **Dynamic Pathfinding:**  
  - Developed advanced navigation algorithms that leverage real-time sensor feedback and probability grids.  
  - Reduced the number of bot actions by 59–79% compared to baseline pathfinding methods.

### Predicting Steps to Locate the Space Rat
- **Data Collection & Modeling:**  
  - Gathered extensive simulation data, including ship layouts, probability grids, and step counts needed to capture the target.
  
- **Deep Learning Integration:**  
  - Built and trained a Convolutional Neural Network (CNN) that uses a two-channel input (ship layout and probability grid) to predict the remaining steps to target capture.  
  - Trained on 1,000 simulation samples over 20 epochs, resulting in a 25% reduction in prediction error and improved decision-making for real-time strategy adjustments.

## Technologies

- **Programming Languages:** Python, C++
- **Libraries & Frameworks:** TensorFlow, PyTorch, Scikit-Learn, OpenCV, MediaPipe, NumPy, Pandas, Matplotlib, Seaborn, Flask, Django
- **Algorithms:** A* Pathfinding, Breadth-First Search (BFS), Probabilistic Modeling, Convolutional Neural Networks (CNNs)

## Project Collaborators

- **Abhishek Jani**
- **Shrey Patel**
- **Mustafa Adil**
