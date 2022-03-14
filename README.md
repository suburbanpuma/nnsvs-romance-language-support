# nnsvs-romance-language-support
Hed and Supporting Files for Romance Language NNSVS Dataset Creation 

This repo contains the files required to create a romance language dataset for use in NNSVS.
Additionally, instructions and examples are provided (or will be provided) for the labeling process.

The phoneme set is custom (somewhat based on arpabet) and has been carefully selected to be as intuitive for native speakers as possible.. A custom phoneme set was chosen over an existing one due to limitations related to differing keyboard layouts and NNSVS/ENUNU compatibility.

Here are the "officially" supported languages so far:
| Language       | Num. Phonemes | Native Spk Verified | est. hours | Dict? |
| -------------- | ------------- | ------------------- | ---------- | ----- |
| Spanish        | 27 ~ 33       | O                   | 1.5 ~ 2.5 hr| O
| BR Portuguese  | 34 ~ 35       | O                   | 2 ~ 3+ hr  |
| EU Portuguese  | 38 ~ 39       | O                   | 2 ~ 3+ hr  |
| Catalan        | 35 ~ 40       | X                   | 1.5 ~ 2 hr |
| Valencian      | 33 ~ 38       | X                   | 1.5 ~ 2 hr |
| Italian        | 28 ~ 34       | O                   | 1.5 ~ 2.5 hr|
| Sicilian       | 33 ~ 34       | X                   | 1.5 ~ 2 hr |
| French         | 34 ~ 36       | O                   | 2 ~ 3+ hr  |
| Belgian French | 34 ~ 35       | O                   | 2 ~ 3+ hr  | ~
| Quebec French  | 36 ~ 37       | O                   | 2 ~ 3+ hr  |
| Ontario French | 36 ~ 38       | ~                   | 2 ~ 3+ hr  | X

Additionally, Ladin and Franco-Provençal support is included but cannot be verified.
More languages are being added but for the initial release, the most "common" languages are supported. If you need support for a romance language that is not listed above, please open an issue.

## Additional Info and Directions

The HED file was written by hand for NNSVS, it may not work in other tools as-is.
Two hed files are included. A minimal and full hed file. Both should work for NNSVS but using the full hed is suggested.

LANG.md files are provided that give descriptions of the phonemes for each language along with examples.

This phoneme set is NOT COMPLETELY COMPATIBLE with Arpabet.
There are several additions/changes that cause the DynamiVox phoneme set to not be 1:1.
However, the basic phoneme section should be about the same.

"DynamiVox Phone Ref.txt" is a cleaned up phoneme document for reference while labeling.

the /dic folder contains several files:  
/romance.conf - phoneme information  
/romance.macron  
/[LANG].table - dictionaries for various lanugages.
/blank.table - basic dictionary for phonetic training (universal for all languages)
/table license.txt - license and source info for dictionaries  

You can change the hed file in config.yaml, this is found at `/train/config.yaml`.

NOTE: please change the value of "in_dim" in `/train/conf/train/*/model/*.yaml`
The values should be set as follows if using "DynamiVox_Romance.hed":

* acoustic_conv.yaml: 389
* acoustic_mdn.yaml: 389
* duration_lstm.yaml: 385
* duration_mdn.yaml: 385
* timelag_ffn.yaml: 385
* timelag_mdn.yaml: 385

Training will not work if these values are incorrect.

A the time of writing, NNSVS doesn't support multi-syllable words in the table. The UST/score will need to be written phonetically.
For phonetic usts, you must use blank.table
Otherwise it may try to match phonemes to pronuncations and fail with `ValueError: could not broadcast input array from shape (###,496) into shape (###,###)`.
