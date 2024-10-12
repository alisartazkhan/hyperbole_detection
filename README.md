# BERT for Hyperbole Classification

Link to paper: https://alisartazkhan.github.io/

Brief description or introduction of the project.

## How to use

* Dataset: Prepare your dataset in a format similar to HYPO.tsv, where each row contains a hyperbolic statement (HYPO) along with its corresponding paraphrases (PARAPHRASES) and minimal units corpus (MINIMAL UNITS CORPUS).
* Training: Run the hyperbole_classification.py script to train the BERT model on your dataset. The script loads the pre-trained BERT model and fine-tunes it for hyperbole classification using the provided dataset. After training, the script evaluates the model on a test dataset and prints the accuracy.
* Inference: You can use the trained model to classify new hyperbolic statements. Use the provided text variable in the script to input your text for classification. The model will output the probability of the input text being hyperbolic and whether it classifies it as hyperbole or not based on a predefined threshold.

## Understanding the Code

* The code first loads the pre-trained BERT model and tokenizer.
* It preprocesses the dataset, splitting it into training, validation, and test sets.
* The model is trained using the training set and evaluated on the validation set for a specified number of epochs.
* After training, the model is evaluated on the test set to calculate the accuracy.
* Finally, the model is used for inference on new text inputs to classify them as hyperbolic or not.

## Customization

* You can adjust the hyperparameters such as learning rate, batch size, and number of epochs for training.
* You can also modify the threshold value used for classifying hyperbolic statements based on your preference.

## Conclusion

* This code provides a simple yet effective way to classify hyperbolic statements using BERT-based models. You can use it as a starting point for building more advanced hyperbole detection systems or integrate it into your applications for identifying exaggerated language.
* I am still working on this project to make improvements.

## References

HYPO is described in the following paper:
* Troiano, E., Strapparava, C., Özbal, G., & Tekiroğlu, S. S. (2018). A Computational Exploration of Exaggeration. In Proceedings of the 2018 Conference on Empirical Methods in Natural Language Processing (pp. 3296-3304).
