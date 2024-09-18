
# TEAM KRISHAK - Irrigation Water Requirement Tool

## Overview

This project helps farmers determine the **irrigation water requirement** for various crops at different growth phases. 
It takes input from the user regarding the crop type and growth phase and provides the corresponding water requirement 
based on a preloaded dataset.

### Features
- **User Input for Crop and Growth Phase:** The tool accepts user inputs for the crop type (e.g., Maize, Cotton) and the growth phase (e.g., Germination, Flowering).
- **Water Requirement Calculation:** Based on the input, the tool cross-references the dataset to retrieve the daily water requirement for the selected crop and phase.
  
### Dataset
The dataset includes the following fields:
- **Crop:** The type of crop (e.g., Maize, Tomato, Cotton).
- **Growth Phase:** The phase of the crop's life cycle (e.g., Germination, Vegetative growth, Harvesting).
- **Water Requirement (mm/day):** The irrigation water needed for each crop in each phase, measured in millimeters per day.

### How to Use

1. **Dataset Loading:**
   The dataset (`crop_data.csv`) is loaded into the tool at the beginning. It includes data for various crops like Maize, Tomato, Groundnut, and Cotton with their water requirements at different growth stages.

2. **User Input:**
   The user is prompted to input the name of the crop and the growth phase. For example:
   ```
   Enter the name of the plant you are growing in the field: Maize
   Enter the phase of the plant you are growing in the field: Germination
   ```

3. **Output:**
   The tool will then display the irrigation water requirement for the selected crop and phase:
   ```
   Irrigation Water Requirement for Maize in Phase Germination: 1.2 mm/day
   ```

   If the entered crop or phase is not found in the dataset, it will inform the user:
   ```
   Plant Maize in Phase Unknown not found in the dataset.
   ```

### Requirements
- **Python** 3.x
- **Pandas** library for data handling.

### Setup

1. Clone or download this repository.
2. Ensure you have Python 3.x installed.
3. Install the required dependencies using pip:
   ```bash
   pip install pandas
   ```
4. Run the notebook or script that uses this logic.

### Example Usage

1. Load the dataset:
   ```python
   df2 = pd.read_csv("crop_data.csv")
   ```
   
2. Input and check the irrigation requirement:
   ```python
   string1 = input('Enter the name of the plant you are growing in the field: ')
   string2 = input('Enter the phase of the plant you are growing in the field: ')
   # ... logic continues
   ```

### License
This project is licensed under the MIT License.
