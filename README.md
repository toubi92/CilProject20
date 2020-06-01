# CIL Project 2020
I have created and ran the jupyter notebook with TensorFlow 2.2 and python 3.6
Bases on a google Colab example about unet: https://www.tensorflow.org/tutorials/images/segmentation

Most arduous was the proper import of the data.
To late I noticed that the training set provides pictures in 400x400, while the actual test set provides pictures in 608x608.
By now I'm applying the 400x400 on the 4 corners of the test image and then merge the predicted masks. But probably we should change the structure of the underlying network anyway.

I have also tried to increase the number of training images by mirroring and flipping the provided image. Interestingly, test scores didn't get any better through that. So I went on and introduced randomness in image characteristics like saturation and brightness, because I think that there is a discrepancy of any such kind between the training set and the test set. Although I got a little better in score, I haven't got a good grip on what's different.

Please have a look at it and share your thoughts. Then I think we should have a skype meeting to discuss how to proceed. If you're interested, we can also step through the jupyter notebook and have a closer look on what's done.

Cheers
