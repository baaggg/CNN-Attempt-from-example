# CNN-Attempt-from-example
Followed Seth Adam's example on YouTube: https://www.youtube.com/playlist?list=PLhA3b2k8R3t2Ng1WW_7MiXeh1pfQJQi_P

Folders / Files in order:

1. clean: My audio files with non-speech removed, and decimated from 48kHz to 16kHz

2. models/conv.model: Directory where the Convolutional Neural Network model and weights were saved

3. pickles: Literally no idea why it's important but it is, check the YouTube playlist from Seth he explains it in the 7th or 8th video
  
4. wavfiles: Raw audio recordings before any decimation, filtering, noise-removal, etc.

5. How I Made TensorFlow2-gpu Work.docx: Word doc I wrote about all the problems I ran into. Has hyperlinked words/sentences so I couldn't copy/paste it to a README file. Any normal person will probably not run into all the same problems I had, but it was good to write down in case this happens again.

6. audiofiles.csv: Made in excel. Just a really basic dataframe used by Pandas to load and save audio files, or do computations on them.

7. cfg.py: Class of different variables used throughout the NN design; some of which are important when exporting/importing a NN model.

8. nn_design.py: The big beautiful file full of TensorFlow and Keras code to design and model the CNN. I barely understand what the hell is happening throughout the code.

9. predictions.py: Script that was supposed to import the model created by nn_design.py, but a KeyError was thrown at line 61: `y_prob = fn_prob[row.fname]` and I'm not smart enough to fix it, nor do I care that much at this time. I would like to believe if that error was not there, the remainder of the code would run correctly. Also sort-of shows how to make a dataframe in Python and use Pandas to export it to a csv file.
