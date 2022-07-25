# AdilRaheem-WeRateDogs-twitter-analysis

# WeRateDogs-twitter-analysis

### Datasets Overview
WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has over 4 million followers and has received international media coverage.<br>
The datasets used for this wrangling project were twitter_archive, api_df, and img_df datasets.<br> 
### Twitter archive dataset
The twitter_archive dataset contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017. Not all data points in the archive were extracted correctly though, this needed to be dealt with in the wrangling steps, which is the sole aim of this project.<br>
### img_df dataset
The img_df dataset contains a table full of image predictions (the top three only) alongside each tweet ID, image URL, and the image number that corresponded to the most confident prediction (numbered 1 to 4 since tweets can have up to four images).
Prediction column and their meanings
-p1 is the algorithm's #1 prediction for the image in the tweet → golden retriever
-p1_conf is how confident the algorithm is in its #1 prediction → 95%
-p1_dog is whether or not the #1 prediction is a breed of dog → TRUE
same goes for p2,p3 and p4 arttributes.<br>

### api_df
The api_df contains additional tweet data including favorite count and retweet count, this data was gathered using Twitter's API.
