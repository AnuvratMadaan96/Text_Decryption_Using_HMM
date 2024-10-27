# Text_Decryption_Using_HMM
This project implements a text decryption system using Hidden Markov Models (HMM) and the Viterbi algorithm. The system is designed to decrypt text that has been encrypted using a simple substitution cipher with jumbled alphabets.

## Overview

The decryption process utilizes the power of Hidden Markov Models to analyze the statistical patterns in the encrypted text and predict the most likely original text. The Viterbi algorithm is employed to efficiently find the most probable sequence of hidden states (in this case, the original characters) given the observed states (the encrypted characters).

## Features

- Decryption of text encrypted with simple substitution cipher
- Implementation of Hidden Markov Model for text analysis
- Utilization of Viterbi algorithm for efficient decryption
- Improved accuracy with longer input texts

## Requirements

- Python 3.x
- NumPy
- SciPy

## Installation

1. Clone this repository:
```bash
git clone https://github.com/AnuvratMadaan96/Text_Decryption_Using_HMM.git
```

2. Navigate to the project directory:
```bash
cd Text_Decryption_Using_HMM
```

3. Install the required dependencies:
```bash
pip install -r requirements.txt
```

4. Run the "main_HMM.ipynb" file:

## How It Works

1. **Initialization**: The HMM is initialized with transition and emission probabilities based on English language statistics.

2. **Training**: The model parameters are refined using the Baum-Welch algorithm on the encrypted text.

3. **Decryption**: The Viterbi algorithm is applied to find the most likely sequence of original characters.

4. **Output**: The decrypted text is generated.

## Usage

You can create a new variable to save your text and add it in the hidden_sequence list.
Now run the main_HMM.ipynb file.

## Performance

Our experiments have shown that the HMM-based decryption performs significantly better with longer input texts. This is due to the increased statistical information available in longer sequences, allowing the model to make more accurate predictions.

## Limitations

- The system assumes that the encryption is a simple substitution cipher.
- Performance may be suboptimal for very short texts or texts with unusual language patterns.

## Contributing

Contributions to improve the decryption algorithm or extend its capabilities are welcome. Please feel free to submit pull requests or open issues for discussion.

## Acknowledgments

- This project was inspired by the work on HMMs in natural language processing.
- Special thanks to the open-source community for providing valuable resources on HMMs and the Viterbi algorithm.
