# eye-typing-data
This repository contains a public database used in experiments for CIKM'16 paper. There are available the following files:

- vc6_filtering2_overlap_min5_thr20.txt: cross validation file with params in given file. Params file has as many line as folds. Each line provides:

> TestPairsFileNameFoldN Pins Pdel Psubs Ptrans Pmatch

Each line of TestPairsFileNameFoldN file contains pairs of input words and expected dictionary words. Pins, Pdel, Psubs, Ptrans, Pmatch are the probability of having insertion, deletion, substitutions, transpositions and matching operations respectively according TestPairsFileNameFoldN. This particular file has 6 folds for each of the six users who participated in our eye-typing experiment.

- pairs_filtering2_overlap_min5_thr20_usuarioN.txt: pairs of input words and expected dictionary words for an user N. These pairs were obtained through an eye-typing experiment with six participants. Gaze positions on the screen were translated into letters on which we applied a high-pass filter with minimum window size of 5 and applying a threshold of 2.0. 

- pairs_filtering2_overlap_min5_thr20_all.txt: all pais of input words and expected dictionary words in a single file

For more information about how these data were obtained, we recommend the lecture of our paper publicated on CIKM'16. Updates will be made soon.
 
