# Twitmap3

Reference:
http://docs.aws.amazon.com/gettingstarted/latest/emr/getting- started-emr-sentiment-create-twitter-account.html
https://gist.github.com/BhavdeepSethi/50f41c6db7b02e2ca94f
#
1. Get the collector program following steps from reference. Simply a listen and save program.
Change the parameter of count(originally it is 500), set the key words to be love. Next put the data to my bucket.
#
2. Run EMR, the reason it fails is
  1.because I don’t have access the the file in tutorial. So I use “$aws s3 cp ”to retrieve files.
  2. The mapper is not corrected.
#
3. Use the mapper program found on github, s3 copy the files to my own bucket. It success. We run the EMR on four collections. With more than 20000 entries, the key word is love.
