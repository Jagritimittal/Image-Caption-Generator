# Image-Caption-Generator
Developed a model to extract image features and applied Natural Language  Processing techniques to generate descriptive captions, enhancing the understanding of images.

# Dataset Used
## Flicker8k_text 
https://drive.google.com/drive/folders/1krZwmJzt8wiMBD8YLzouFUX0HP-ODcq9?usp=sharing
## Flicker8K_Dataset
https://drive.google.com/drive/folders/14YJyqPviidcuSVxEsckAGttiPKHXkkwH?usp=drive_link

The dataset consists of 8091 images, stored in the Flicker8k_Dataset folder. Accompanying text files with image captions are located in the Flickr_8k_text folder. The Flickr8k.token file, lists all image names alongside their corresponding captions. 

# Image Caption Generator Model 
Image Caption Generator Model = CNN + LSTM

1. CNN - To extract features from the image.
2. LSTM - To generate a description from the extracted information of the image.

# Data Preprocessing Techniques
## Removed Stop Words
Stop words, which are common and generally insignificant words, were removed from the captions to enhance model efficiency.

## Converted to Lower Case
All text was converted to lower case to ensure uniformity and prevent treating words with different cases as distinct tokens.

## Removed Punctuation
Punctuation was stripped to simplify the data and reduce the complexity of the vocabulary.

## Saved Cleaned Descriptions
The cleaned and processed descriptions were saved in a file (e.g., descriptions.txt) to avoid repeating preprocessing steps and to facilitate easy loading for model training.

# NLP Techniques
## Tokenized
Broke down captions into individual words or tokens, which was essential for creating a structured form of text data that the model could analyze and process.

## Created Vocabulary from Tokenized Words
Created a vocabulary list of all unique words in the dataset. This list was used to map words to indices, which was crucial for the model's understanding and generation of captions.
