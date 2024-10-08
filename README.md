# Sentiment-Analysis-of-Restaurant-Reviews



## Project Purpose
This project demonstrates the integration of Hugging Face's sentiment analysis models with Gradio to classify restaurant reviews and visualize review ratings. Users can submit a restaurant review and receive a predicted rating, a classification of the review's sentiment (positive or negative), and an accuracy score.

## Main Files
- **Restaurant_reviews.csv**: This file contains the restaurant reviews and corresponding ratings.
- **full_review_sentiment_analysis.py**: This Python script integrates fuzzy matching and sentiment analysis using Gradio for interactive review classification and plotting rating distribution.
- **gradio_review_classifier.py**: This Python file focuses on building a simple Gradio interface for classifying reviews and displaying a plot of rating distribution.
- **basic_sentiment_analysis.py**: This Python file demonstrates a basic example of sentiment analysis using the Hugging Face model.

## How Hugging Face's Sentiment Analysis Works
The project utilizes Hugging Face’s pipeline API to perform sentiment analysis. It uses the (`distilbert-base-uncased-finetuned-sst-2-english`) model to classify text as either positive or negative.

python
```bash
classifier = pipeline('sentiment-analysis', model='distilbert-base-uncased-finetuned-sst-2-english')
```

For example:
python
```bash
result = classifier("The food was great!")
```

This would return a sentiment classification with a confidence score.

## How to Run:
1. Clone the repository:
   ```bash
   git clone https://github.com/Almahfouz/Sentiment-Analysis-of-Restaurant-Reviews
   ```
   After running this command navigate the folder that you have save the repository at, then run *full_review_sentiment_analysis.py* file

## Expected Output

### Review Classifier
Input a review, and the classifier will return:
- A rating-based classification from the dataset.
- A sentiment analysis result from the Hugging Face model.
  
As shown in the figure below:
![image](https://github.com/user-attachments/assets/1ae9378e-b818-420a-bdfb-f964700c77f2)


### Rating Distribution
![image](https://github.com/user-attachments/assets/b99b659c-82d0-4be3-af6b-102e8be43994)


### Dataset Preview
![image](https://github.com/user-attachments/assets/a0258d71-ce5d-4538-9bf6-cc51ae78fa84)


## Hugging Face Project Page

- [Hugging Face Project](https://huggingface.co/spaces/Almahfouz/Sentiment-Analysis-of-Restaurant-Reviews-Using-Hugging-Face-and-Gradio)

## Video 
link video: -[Drive](https://drive.google.com/file/d/1-YvZywKkpaPLN-N_9t55i86-GrWdBSrO/view?usp=sharing)

## Dataset Link
-[Kaggle](https://www.kaggle.com/datasets/joebeachcapital/restaurant-reviews)
