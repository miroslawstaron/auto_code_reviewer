# Auto_code_reviewer
Automated support for code reviews. 

## Explanation of the components:
* gerrit_exporter_loop_comments.ipynb -- jupyter notebook that exports a raw data from a gerrit repository; results in a .csv file with the comments and the commented lines
* review_comments_to_sentiment.ipynb -- jupyter notebook that takes the file exported from gerrit and analyzes the sentiment of the comments. The output of this workbook is each line with it's class, based on the sentiment (0- "bad line" and 1 - "ok")
* bow_featurizer.ipynb -- jupyter notebook with the code to create a bag of words representation of the code 
* classification -- jupyter notebook with the code for training the classifier