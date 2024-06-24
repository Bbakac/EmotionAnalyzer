# EmotionAnalyzer Project

## Project Overview
This project aims to analyze emotions from Twitter data using a dataset from Kaggle. The data is categorized into five different emotions: Angry, Fear, Happy, Surprise, and Sad. The project involves collecting data from Twitter, processing and analyzing it to detect emotions, and visualizing the results on a web interface.

## Repository Link
You can access the project repository on GitHub [here](https://github.com/Bbakac/EmotionAnalyzer.git).

## Goals
- **Data Collection:** Gather a large dataset of tweets using the Twitter API.
- **Emotion Labeling:** Manually or automatically label the collected tweets with corresponding emotions.
- **Model Development:** Develop and train a machine learning model for emotion analysis using the labeled dataset.
- **Web Interface:** Design a user-friendly web interface to visualize the results of the analysis.

## Dataset Description
The dataset contains over 10,000 entries, with the following columns:
- **Tweets:** The content of the tweet.
- **Search key:** The search keyword used to collect the tweet.
- **Feeling:** The labeled emotion of the tweet.

## Data Preprocessing
The data preprocessing steps include:
- Removing special characters.
- Converting text to lowercase.
- Removing unnecessary spaces.

## Model Development
The following steps were taken to develop the emotion analysis model:
- **Vectorization:** Using CountVectorizer and TfidfVectorizer to convert text data into numerical vectors.
- **Training and Testing Split:** Dividing the dataset into training and testing sets using `train_test_split`.
- **Model Training:** Using a DecisionTreeClassifier to train the model.
- **Evaluation:** Assessing the model's performance with accuracy score, confusion matrix, and classification report.

## Methods Used
- **Pandas and NLTK:** For data analysis and preprocessing.
- **Seaborn and Matplotlib:** For data visualization.
- **Scikit-learn:** For machine learning model development and evaluation.

## Web Interface
The results are visualized through a web interface built with HTML and CSS. The interface includes:
- **Index Page:** An introductory page with a button linking to the results.
- **Results Page:** An embedded iframe displaying the detailed project report and analysis results.

## Key Files
- **app.py:** The main application file for running the web interface.
- **data.csv:** The dataset used for the analysis.
- **index.html:** The homepage of the web interface.
- **results.html:** The page displaying the analysis results.
- **Berkay_Bakaç_Bitirme_Ödevi_Raporu_Final.pdf:** The final project report detailing the methodology and findings.

## How to Run
Follow these steps to set up and run the project on your local machine:

### Prerequisites
Ensure you have the following installed:
- **Python 3.7 or higher**
- **pip** (Python package installer)

### Installation Steps

1. **Clone the repository:**
    ```sh
    git clone https://github.com/Bbakac/EmotionAnalyzer.git
    cd EmotionAnalyzer
    ```

2. **Create a virtual environment:**
    ```sh
    python -m venv env
    ```

3. **Activate the virtual environment:**
    - On Windows:
        ```sh
        .\env\Scripts\activate
        ```
    - On macOS and Linux:
        ```sh
        source env/bin/activate
        ```

4. **Install the required libraries:**
    ```sh
    pip install -r requirements.txt
    ```

### Running the Project

1. **Run the application:**
    ```sh
    python app.py
    ```

2. **Open your browser and go to:**
    ```sh
    http://127.0.0.1:5000/
    ```

You should now see the web interface with options to view the analysis results.

## Requirements
Here is the content of the `requirements.txt` file listing all the necessary Python libraries:
```txt
Flask==2.0.1
nltk==3.6.2
numpy==1.21.0
pandas==1.3.0
scikit-learn==0.24.2
seaborn==0.11.1
matplotlib==3.4.2



## Conclusion
This project successfully demonstrates the process of collecting, processing, and analyzing Twitter data for emotion detection. The developed model and web interface provide valuable insights into the emotional states expressed on Twitter.
