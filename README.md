# Sri Lankan Travel Recommendation System

This project is a travel recommendation system designed to suggest the best places to visit in Sri Lanka based on user preferences and activities. The system leverages machine learning techniques to deliver personalized travel recommendations.

---

## Table of Contents

- [Overview](#overview)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Project Structure](#project-structure)  
- [Data](#data)  
- [Model](#model)  
- [Contributing](#contributing)  
- [License](#license)  

---

## Overview

The Sri Lankan Travel Recommendation System analyzes user profiles and destination data to generate customized travel recommendations. Users can receive suggestions tailored to their preferences, including favorite activities and bucket list destinations. 

The system is built using TF-IDF vectorization and cosine similarity to match user interests with travel locations. The modular structure ensures flexibility and scalability for additional features.

### Model Architecture
![download](https://github.com/user-attachments/assets/ea6771f9-c590-485b-8c69-0c420c27ec54)

---

## Installation

To set up the project locally:  

1. Ensure **Python 3.11.3** or later is installed.  
2. Clone this repository.  
3. Install the required packages using the following command:

    ```bash
    pip install -r requirements.txt
    ```

---

## Usage

Follow these steps to use the travel recommendation system:

1. **Prepare Data**  
   Ensure the following files are present in the project directory:
   - `places_preprocessed.csv`  
   - `users_preprocessed.csv`  

2. **Run the Notebook**  
   Open and execute the `Final Notebook.ipynb` to load the recommendation model and generate travel suggestions.

3. **Input User Preferences**  
   Modify the `user_number` variable in the notebook to select a specific user profile for recommendations.

4. **View Recommendations**  
   The notebook will display the user's preferred activities, bucket list destinations, and the final recommended travel locations.

---

## Project Structure

```plaintext
Sri Lankan Travel Recommendation System/
├── Final Notebook.ipynb            # Main notebook for running the system
├── Model checking.ipynb            # Validation and testing of the recommendation model
├── Pre processing.ipynb            # Data preprocessing notebook (currently empty)
├── Additional_model_with_NN/
│   └── Sri Lankan Travel Recommendation System.ipynb  # Additional model implementation
├── data/
│   ├── places_preprocessed.csv     # Data about places in Sri Lanka
│   └── users_preprocessed.csv      # User profile data
├── Recommendation Model.pkl        # Serialized recommendation model
├── Model Architecture   
└── Project documentation 
```

---

## Data

- **Places Data (`places_preprocessed.csv`)**  
  Contains details of tourist destinations in Sri Lanka, such as activities, features, and highlights.  

- **User Data (`users_preprocessed.csv`)**  
  Profiles of users including preferences for activities and bucket list destinations.  

---

## Model

The recommendation system employs:  
- **TF-IDF Vectorization**: To quantify textual data on user preferences and destinations.  
- **Cosine Similarity**: To identify the best matches between user profiles and travel destinations.

The trained model is serialized as `Recommendation Model.pkl` and is loaded using the `dill` library for seamless use in the notebooks.

---

## Contributing

Contributions are encouraged! To contribute:

1. Fork the repository.  
2. Create a feature branch: `git checkout -b feature-name`.  
3. Commit your changes: `git commit -m 'Add feature description'`.  
4. Push to the branch: `git push origin feature-name`.  
5. Open a pull request to the main branch.

---

## License

This project is licensed under the **MIT License**. Refer to the `LICENSE` file for further details.

---
