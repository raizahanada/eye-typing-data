# eye-typing-data
This repository contains the files used in experiments for the CIKM'16 paper entitled "Effective Spelling Correction for Eye-based Typing using domain-speciﬁc Information about Error Distribution". The included files are:

- vc6.txt: file with information for cross validation. The n-th line provides information related to the n-th fold. Fields are separated by spaces as follows:

> TestPairsFileNameFoldN Pins Pdel Psubs Ptrans Pmatch

where TestPairsFileNameFoldN is the name of the text file which contains the pairs <input word, dictionary word> (see below). Pins, Pdel, Psubs, Ptrans, Pmatch correspond to insertion, deletion, substitution, transposition and matching probabilities for the specific training-test split. This particular file (vc6_filtering2_overlap_min5_thr20.txt) describes 6 folds, one for each of the six users who participated in our eye-typing experiment.

- pairsN.txt: text file which contains the pairs <input word, dictionary word> of the N-th user. Each line corresponds to a pair, with words separated by space as in the following example:

> lojvde love

where "lojvde" corresponds to the word typed by the user and "love" corresponds to the dictionary word the user intended to type. These pairs were obtained through an eye-typing experiment with six participants. Gaze positions on the screen were translated into letters after applying a high-pass filter. 

- pairsall.txt: all pairs <input word, dictionary word> related to all users, in a single file.

For additional information about this data, we refer the reader to our CIKM'16 paper entitled "Effective Spelling Correction for Eye-based Typing using domain-speciﬁc Information about Error Distribution". 


