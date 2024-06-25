# predict-hand-movement-eeg
Code on reading EEG data to predict hand movements of people.
Using EEG data from various users with varying hand movements, let's attempt to predict the user and hand movement of a given reading.

To create our predictions, a TensorFlow neural network will be utilised. 

1. Goal: Predict hand movements from EEG data using machine learning.
2. Data: EEG recordings from 4 users, including electrode readings (AF3, AF4, F7, etc.) for various brainwave types (delta, theta, alpha, beta)
3. Preprocessing: One-hot encoding, train-test split (70-30), StandardScaler for feature scaling.
4. Model: Neural network with 2 hidden layers (128 neurons, ReLU), output layer (3 neurons, softmax).
5. Training: Adam optimizer, sparse categorical cross-entropy loss, 50 epochs max with early stopping.
6. Performance: ~65% accuracy for hand movement prediction, ~100% for user identification.
7. Implementation: Python, using pandas for data handling, sklearn for preprocessing, and TensorFlow for the neural network.
8. Key challenge: Balancing model complexity with performance for multi-user EEG data.
9. Potential application: Controlling prosthetics for paralyzed individuals.
