# Detection of Hate Speech Against LGBT+ on Social Media

This project aims to detect potential hate speech targeting people of the LGBTQIA+ community.
The model is trained using a supervised learning approach, where it learned patterns from labeled data to make predictions on unseen text. For the training of the model ,a dataset containing examples of hate speech and non-hate speech texts related to LGBTQIA+ topics was used.

The project uses key concepts of Natural Language Processing, employs TF-IDF for the vectorization of the text.

For the preprocessing of the text, basic operations like removing URLS,Stop Words, Punctuation marks,Digits was done, followed by tokenization and lemmatization. 
Post this, frequencies of the most repeating words were plotted on wordclouds.
![Screenshot (366)](https://github.com/parth9504/Hate-Speech/assets/127659489/90dfd7b8-7a19-40d9-b68c-8f385a4246f8)
![Screenshot (367)](https://github.com/parth9504/Hate-Speech/assets/127659489/93d7ad37-6789-47d0-964c-98ddd409fa19)

TF-IDF (Term Frequency-Inverse Document Frequency) vectorization was used in this project to convert text into numerical features. TF-IDF assigns weights to words based on their frequency in a document relative to their frequency in the entire corpus, helping capture the importance of words in a document.

For the classification, Random Forest was used, which is an ensemble learning method that builds multiple decision trees during training and combines their predictions to make a final prediction.

The project not only provides predictions of hate speech from user input (in the form of text) but also allows scraping of tweets and comments from a YouTube video, as well as uploading CSV files. For scraping tweets, the Python library ntscraper was used, while for YouTube comments, the YouTube API was utilized.
Streamlit library was used to build and design the user interface.

Refer to the attached screenshots demonstrating the working of the project.
![Screenshot (368)](https://github.com/parth9504/Hate-Speech/assets/127659489/0f7db914-d4ba-45ed-a13d-3be64d07408e)
![Screenshot (369)](https://github.com/parth9504/Hate-Speech/assets/127659489/3b91cbc1-5165-4739-81e1-c7fafff05239)

The "Youtube Comments Analysis" section allows the users to enter any valid link of a youtube video and scrape the comments to make predictions on that data. The same is displayed on the screen.

![Screenshot (370)](https://github.com/parth9504/Hate-Speech/assets/127659489/946b6541-56db-4f2d-a87e-48a934f67434)

The "File Upload" section allows the users to import any csv file which has a 'text' column in it.The textual data is then analysed for the presence of hate speech and the same is then displayed on the screen.

![Screenshot (371)](https://github.com/parth9504/Hate-Speech/assets/127659489/16c6f783-d258-4d87-9b1c-e9d61aec2136)

The "Tweets Analysis" section provides the feature of using a term or a valid twitter username, to scrape tweets and make predictions on the scraped data.

![Screenshot (372)](https://github.com/parth9504/Hate-Speech/assets/127659489/96e99c1a-9481-4a84-91f9-94f8587e941f)
