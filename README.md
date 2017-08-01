# InvisiBoard
Top 10 at Greylock Hackfest 2017. Uses OpenCV along with some fundamental
natural language processing to turn any smartphone and any surface into a
keyboard.

OpenCV: calculates the length of each finger and tracks them, turning the jerks of each finger (change in length) into keypresses. We used IP Webcam to stream video to OpenCV. 

Autocorrect: takes each character returned from the image recognition to construct a word, then autocorrects the word and displays the corrected word to the user. We generated frequency distributions from large NLTK corpuses as well as used a modified edit distance algorithm tailored to the errors that would be made in our application. Additionally, we used some Bayesian analysis of a corpus of novels, news, and other texts to selectively promote words.

Pynput: using Pynput, we were able to have the keyboard output to any valid text field, showing the feasibility of the prototype as a general-use keyboard.
