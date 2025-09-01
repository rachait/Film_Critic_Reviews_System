# Film Critic Reviews Sentiment Analysis using LSTM

A deep learning project that uses Long Short-Term Memory (LSTM) neural networks to perform sentiment analysis on movie reviews from the IMDB dataset.

## 🎬 Project Overview

This project implements a sentiment analysis model that can classify movie reviews as either **positive** or **negative**. The model is trained on 50,000 movie reviews from the IMDB dataset and achieves an accuracy of approximately **87.89%** on the test data.

## 🚀 Features

- **Deep Learning Model**: Uses LSTM (Long Short-Term Memory) neural networks
- **Large Dataset**: Trained on 50,000 IMDB movie reviews
- **High Accuracy**: Achieves ~87.89% accuracy on test data
- **Real-time Prediction**: Can predict sentiment of new movie reviews
- **Text Preprocessing**: Includes tokenization and sequence padding
- **Easy to Use**: Simple prediction function for new reviews

## 📊 Dataset

- **Source**: IMDB Dataset of 50K Movie Reviews
- **Size**: 50,000 reviews
- **Classes**: Binary (Positive/Negative)
- **Split**: 80% training, 20% testing
- **Format**: CSV file with review text and sentiment labels

## 🏗️ Model Architecture

- **Embedding Layer**: 5000 vocabulary size, 128 dimensions
- **LSTM Layer**: 128 units with dropout (0.2) and recurrent dropout (0.2)
- **Dense Layer**: 1 unit with sigmoid activation
- **Optimizer**: Adam
- **Loss Function**: Binary crossentropy

## 📋 Requirements

- Python 3.7+
- TensorFlow/Keras
- pandas
- scikit-learn
- kaggle
- numpy

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/film-sentiment-analysis-lstm.git
   cd film-sentiment-analysis-lstm
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up Kaggle API**
   - Create a Kaggle account and generate API credentials
   - Place your `kaggle.json` file in the project directory
   - The notebook will automatically use these credentials to download the dataset

## 📖 Usage

### Running the Jupyter Notebook

1. **Start Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

2. **Open the notebook**
   - Navigate to `Film_Critic_reviews_Sentiment_Analysis_LSTM (1).ipynb`
   - Run all cells sequentially

### Using the Prediction Function

After training the model, you can predict sentiment for new reviews:

```python
# Example usage
new_review = "This movie was fantastic. I loved it!"
sentiment = predict_sentiment(new_review)
print(f"The Sentiment of the review is: {sentiment}")
```

## 📈 Results

- **Training Accuracy**: ~93.63% (final epoch)
- **Validation Accuracy**: ~87.27% (final epoch)
- **Test Accuracy**: ~87.89%
- **Test Loss**: 0.342

### Training Progress
- **Epoch 1**: 81.17% training accuracy, 87.02% validation accuracy
- **Epoch 2**: 89.22% training accuracy, 87.14% validation accuracy
- **Epoch 3**: 90.99% training accuracy, 87.08% validation accuracy
- **Epoch 4**: 92.29% training accuracy, 87.64% validation accuracy
- **Epoch 5**: 93.63% training accuracy, 87.27% validation accuracy

## 🔍 Example Predictions

| Review | Predicted Sentiment |
|--------|-------------------|
| "This movie was fantastic. I loved it!" | Positive |
| "The film's stunning visuals and compelling storyline make it a must-watch." | Positive |
| "This movie ok but not that good." | Negative |
| "The movie's plot was convoluted and hard to follow, leaving me disappointed." | Negative |

## 📁 Project Structure

```
film-sentiment-analysis-lstm/
├── Film_Critic_reviews_Sentiment_Analysis_LSTM (1).ipynb
├── README.md
├── requirements.txt
├── kaggle.json (you need to add this)
├── IMDB Dataset.csv (downloaded automatically)
└── imdb-dataset-of-50k-movie-reviews.zip (downloaded automatically)
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Dataset**: IMDB Dataset of 50K Movie Reviews by Lakshmi25npathi on Kaggle
- **Framework**: TensorFlow and Keras for deep learning implementation
- **Platform**: Kaggle for dataset hosting and API access

## 📧 Contact

If you have any questions or suggestions, feel free to reach out:

- **GitHub**: [yourusername](https://github.com/yourusername)
- **Email**: your.email@example.com

---

⭐ If you found this project helpful, please give it a star on GitHub!
