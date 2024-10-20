Federated Learning & Differential Privacy with Blockchain Integration

Introduction

This project combines the principles of federated learning, differential privacy, and blockchain technology to create a privacy-preserving, secure, and decentralized machine learning architecture. The aim is to demonstrate how sensitive data can be analyzed and processed across multiple locations without compromising privacy, using differential privacy mechanisms and secure blockchain nodes for validation, storage, and computation.

Features

Differential Privacy: Utilizes the Laplace mechanism to add noise, ensuring that private data is protected while still enabling statistical analysis.
Federated Learning: Trains models locally on decentralized datasets, aggregates the models, and generates a central model without sharing raw data.
Blockchain Nodes: Implements different types of nodes (validator, storage, and compute) to simulate secure data transactions and decentralized processing.
Customizable Parameters: Users can easily modify privacy levels, features, and model configurations to explore different setups and observe the impact on results.
Performance Visualization: Automatically generates plots to analyze how various privacy settings impact metrics such as accuracy, precision, recall, processing time, and privacy loss.
Getting Started
Prerequisites
Make sure you have the following Python packages installed:

numpy
pandas
matplotlib
scikit-learn
tracemalloc
You can install the dependencies using:

bash
Copy code
pip install numpy pandas matplotlib scikit-learn
File Structure
federated_privacy_blockchain.py: The main script containing the complete code.
BankCustomerData.csv: Example dataset used for training and testing.
README.md: Detailed explanation of the project.
Data Requirements
The script expects a CSV file named BankCustomerData.csv with the following structure:

Feature Columns: age, balance, duration, campaign, previous
Target Column: term_deposit (values should be yes or no)
Feel free to modify the script to work with your custom dataset by updating the feature_columns and target_column variables.

How to Run
Place your dataset (or use the sample dataset) in the same directory as the script.
Modify the configurable section at the beginning of the code to adjust parameters like epsilon, feature columns, and more.
Run the script using:

bash:

pip install numpy pandas matplotlib scikit-learn

Run the script using:

python federated_privacy_blockchain.py

The script will train models, simulate privacy-preserving transactions, and generate visual outputs.
Configuration Options
1. Privacy Settings
Adjust the epsilon_values to explore different levels of privacy. Lower epsilon means higher privacy but may introduce more noise, affecting accuracy.

python

epsilon_values = [0.1, 0.5, 1.0, 5.0, 10.0]

2. Feature and Target Selection
Customize the features and target column according to your dataset.

python

feature_columns = ['age', 'balance', 'duration', 'campaign', 'previous']
target_column = 'term_deposit'

3. Node Configuration
Modify or add new blockchain nodes to simulate different roles within the network.

python

node1 = Node('validator', 1)
node2 = Node('storage', 2)
node3 = Node('compute', 3)
Output
The script will generate the following:

Performance Metrics: Including accuracy, precision, recall, processing time, memory usage, privacy loss, and entropy.
Visualizations: Graphs showing the impact of epsilon on model accuracy, privacy loss, and other metrics.
Example Visualizations
After running the script, you will see visualizations like:

Mean Error & Sum Error vs. Epsilon: Understand how privacy impacts aggregate values.
Accuracy, Precision & Recall vs. Epsilon: Analyze model performance under different privacy conditions.
Processing Time & Memory Usage vs. Epsilon: Observe resource consumption.
Privacy Loss & Entropy vs. Epsilon: Track the trade-offs between privacy and data utility.
Contributing
Feel free to fork this repository, make improvements, and submit pull requests. Contributions are always welcome!

License
This project is open-source and free to use under the MIT License.

Contact
For questions, suggestions, or feedback, please contact:

Email: nastaranbeiranvand1994@gmail.com
GitHub:(https://github.com/Drnastaran)
