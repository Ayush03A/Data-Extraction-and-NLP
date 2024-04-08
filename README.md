Instructions
Here's the explanation of the provided Python script, including how to run it, and the dependencies required:

Link of colab : https://colab.research.google.com/drive/1PFolDMuYbIphIp-QxVX3oZ-huZG-6Za8

Approach to the Solution:

1.The script begins by importing necessary libraries such as pandas, requests, BeautifulSoup, nltk, and os.
2.It defines paths for input CSV, output text files, positive and negative words lists, stop words, and output Excel file.
3.A function scrape_article is defined to scrape article titles and text from given URLs using BeautifulSoup and requests.
4.Another function save_to_txt is defined to save scraped article title and text to text files.
5.A clean_text function is defined to remove stop words from the text.
6.A textual_analysis function is defined to perform textual analysis including word tokenization, removing stop words, calculating word frequency, polarity score, subjectivity score, etc.
7.The input CSV is read using pandas and iterated row by row to scrape articles, clean text, and perform textual analysis.
8.Output data is stored in a pandas DataFrame.
9.Finally, the output DataFrame is saved to an Excel file.

Running the .py File:

1.Make sure to have Python installed on your system along with required libraries (pandas, nltk, requests, BeautifulSoup, etc.).
2.Set the correct paths for input CSV, output text files, positive and negative words lists, stop words, and output Excel file.

Dependencies:

●Python (>=3.6)
●Pandas
●Requests
●BeautifulSoup
●nltk

You need to ensure that the necessary libraries are installed in your Python environment. You can install them using pip.
