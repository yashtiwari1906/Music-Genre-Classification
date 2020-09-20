# Music-Genre-Classification

Music genre classification from audio spectrograms using deep learning A convolutional neural network is trained with 1000 sample audios of 6 different music genres.

GENRES: classical - hiphop - jazz - metal - pop - reggae

# Preprocessing 
All the audio dataset is converted into mel - spectograms so that this problem can be solved with the help of CNN, prepare_data() will generate your required dataset with the help of mel_spectogram()(which will convert a audio sample to mel-spctogram) and list_mel_spectogram()(which generate data set for a particular split for eg. train,test and validation.

# Model
we a have a shallow CNN model in which input shape will be (64,2584,1) optimizer is Adam and metrics used is accuracy we obtained test accuracy of 75% approx. one noticable thing from confusion matrix is model is finding difficulty in classifying hipop and reggae may be because beats used in both music is of same pattern. we had saved our model as a json file and also saved its weight as model.h5.

# Testing on real world music
we are taking audio from get_audio() and preprocessing it to obtain mel-spectogram then we are predicting it which is shown with the help of a plot.
the music is taken from - https://www.youtube.com/watch?v=312Sb-2PovA
![alt text](https://github.com/yashtiwari1906/Music-Genre-Classification/blob/master/Images/plot_.jpeg)
