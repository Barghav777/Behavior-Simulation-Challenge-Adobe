# Adobe Behavior Simulation Challenge
This repository contains our team's solution to the Adobe Behavior Simulation Challenge, developed as part of an internal hackathon for the selection process in Inter IIT 2024.

## Problem Statement
The challenge includes two primary tasks:
1. **Behavior Simulation**: Predicts user engagement (number of likes) on tweets based on tweet content, media type, company, username, and timestamp. 
2. **Content Simulation**: Generates potential tweet content based solely on metadata (company, username, media type, timestamp).

## Approach
### Task 1: Behavior Simulation
- **Objective**: Predict engagement levels for social media posts.
- **Model Pipeline**:
  - **Feature Extraction**: Processed metadata, media captions, and timestamps to create a feature-rich dataset.
  - **Model**: Used XGBClassifier for initial classification into engagement categories, followed by a regression layer to refine engagement predictions.
- **Evaluation**: RMSE

### Task 2: Content Simulation
- **Objective**: Generate tweet content from metadata alone.
- **Model Pipeline**:
  - **Metadata Extraction**: Collected structured tweet metadata to use as input features.
  - **Text Generation**: Used models like BLIP-2 to generate media captions and fine-tuned BART model for tweet reconstruction.
- **Evaluation**: BLEU, ROGUE, CIDEr

## Repository Structure
- `Behaviour_Simulation_Challenge_Task1/` - Folder containing files for Behavior Simulation.
- `Behavior_Simulation_Challenge_Adobe_Task2/` - Folder containing files for Content Simulation.

### Installation
Clone the repository:
   ```bash
   git clone https://github.com/Barghav777/Behavior-Simulation-Challenge-Adobe.git
   cd Behavior-Simulation-Challenge-Adobe
```

## Team
- [HIMANSHU](https://github.com/him-a-n-shu)
- [D Barghav](https://github.com/Barghav777)
- Purushartha Gupta
- Aman Nagar
- Palak
- Misti D Shah
