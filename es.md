Cleaned up reference provided by Subpum

|   | Type    |
| - | ------- |
| C |Consonant|
| V |Vowel    |
| S |Semivowel|

## Other:

| Phoneme | X-SAMPA | Description |
| ------- | ------- | ----------- |
| br      |         | Inhale      |
| exh     |         | Exhale      |
| axh     |         | Voiced exhale|
| pau     |         | Silence     |
| q       | ?       | Glottal Stop|
| cl      |         | closure (held consonants) |
| vf      |         | Vocal Fry   |
| trash   |         | junk phoneme| 

## Vowels:

| Phoneme | X-SAMPA | Explaination                    | Example                                 |
|---------|---------|---------------------------------|-----------------------------------------|
| a       | a       | central open unrounded vowel    | <ins><b>A</ins></b>n<ins><b>a</ins></b> |
| e       | e       | close-mid front unrounded vowel | <ins><b>E</ins></b>va                   |
| i       | i       | close front unrounded vowel     | L<ins><b>i</ins></b>nda                 |
| o       | o       | close-mid back rounded vowel    | T<ins><b>o</ins></b>pe                  |
| u       | u       | close back rounded vowel        | <ins><b>U</ins></b>no                   |

## Semi-Vowels:
(Semi-vowels function as consonants and perfrom "diphthong-like" tasks.)
| Phoneme | X-SAMPA | Explaination                    | Example                                 |
|---------|---------|---------------------------------|-----------------------------------------|
| y       | j       | palatal approximant      | A<ins><b>i</ins></b>re (a <ins><b>y</ins></b> r e), t<ins><b>i</ins></b>erra (t <ins><b>y</ins></b> e rr a), sa<ins><b>y</ins></b>o (s a <ins><b>y</ins></b> o) |
| w       | w       | labial-velar approximant | Pa<ins><b>u</ins></b>sa (p a <ins><b>w</ins></b> s a), f<ins><b>u</ins></b>ego (f <ins><b>w</ins></b> e gg o)                                                   |

Consonants:

| Phoneme | X-SAMPA | Explanation                        | Example                   |
|---------|---------|------------------------------------|---------------------------|
| b       | b       | voiced bilabial plosive            | <ins><b>b</ins></b>año (<ins><b>b</ins></b> a ny o)           |
| bh      | B       | voiced bilabial fricative          | abaco (a bh a k o)        |
| ch      | tS      | voiceless postalveolar affricate   | choripan (ch o r i p a n) |
| d       | d       | voiced alveolar plosive            | día (d i a)               |
| dh      | D       | voiced dental fricative            | andina (a n dh i n a)     |
| f       | f       | voiceless labiodental fricative    | farol (f a r o l)         |
| g       | g       | voiced velar plosive               | gato (g a t o)            |
| gh      | G       | voiced velar fricative             | agua (a gh w a)           |
| k       | k       | voiceless velar plosive            | casa (k a s a)            |
| l       | l       | lateral alveolar approximant       | lame (l a m e)            |
| ll      | L       | voiced palatal lateral approximant | pollo (p o ll o)          |
| m       | m       | bilabial nasal                     | madre (m a d r e)         |
| n       | n       | alveolar nasal                     | nadie (n a d j e)         |
| ny      | J       | palatal nasal                      | ñoquis (ny o k i s)       |
| p       | p       | voiceless bilabial plosive         | puerta (p w e r t a)      |
| r       | 4       | alveolar flap                      | larga (l a r g a)         |
| rr      | r       | alveolar trill                     | rara (rr a r a)           |
| s       | s       | voiceless alveolar fricative       | suena (s w e n a)         |
| sh      | S       | voiceless postalveolar fricative   | show (sh o w)             |
| t       | t       | voiceless alveolar plosive         | tema (t e m a)            |
| x       | x       | voiceless velar fricative          | jamón (x a m o n)         |
| y       | j\      | voiced palatal fricative           | yace (y a s e)            |
| z       | T       | voiced alveolar fricative          | zeta (z e t a)            |


## Dialect Allophones:
READ THE NOTES for how to handle these.

| Phoneme | X-SAMPA | Explanation                           | Example               | Dialect                                               |
|---------|---------|---------------------------------------|-----------------------|-------------------------------------------------------|
| ts      | ts      | voiceless alveolar sibilant affricate | chala (ts a l a)      | Reference allophone for ch.                           |
| zh      | Z       | voiced postalveolar fricative         |                       | Reference allophone for ch.                           |
| sh      | S       | voiceless postalveolar fricative      | chala (sh a l a)      | Reference allophone for ll/ch.                        |
| h       | h       | voiceless glottal fricative           | obispo (o bv i h p o) | Reference allophone for s/x.                          |
| v       | v       | voiced labiodental fricative          | afgano (a v gh a n o) | Reference allophone for f (before voiced consonants). |
| dj      |         |                                       |                       | Reference allophone for g (before some vowels).       |
| ng      | N       | velar nasal                           | dingo (d i ng g o)    | Reference allophone for n (before velar consonants).  |


Notes:
* `sh` and `zh` are sometimes used as allophones for `ll`. Still label it as `ll` for dictionary compatiblity. However, these phonmemes are useful for foreign words.
  
* Some speakers enounter "yeísmo", or the merging of "ll" and "y". These speakers can label "ll" as `y` instead to slightly reduce the amount of training data needed.
  
* Some speakers merge the hard and soft "b/d/g" sounds. These speakers can label all "b/d/g" as [`b`/`d`/`g`] and ignore the [`bh`/`dh`/`gh`] phonemes. Speakers without this merger can also drop [`bh`/`dh`/`gh`] to simplify the dataset, which will cause most "b/d/g” instances to sound softer (due to more instances of the soft sound in speech). Doing so also creates a slight risk that the model may use a hard "b/d/g" at an incorrect time.
  
* The `y` phoneme works as both a consonant AND semivowel. This is thanks to NNSVS being able to learn context.
  
* `x` covers all "h/soft J/aspirated s" sounds contextually. So only one phoneme is required. For speakers who want to differentiate, the `h` phoneme could be used along with the others. Note that this will increase the amount of data required and won't be supported in the dictionary.

* `f` is used for both devoiced "f" and voiced "v" sounds.

Chilean speaker notes: 
* Upper-class speakers use `ts` instead of `ch`.
* Lower-class speakers use `sh` instead of `ch`.
* In most cases you should still label these as `ch` for dictionary compatiblity. Only differenciate if the speaker between `ts`/`sh` and `ch` (optional).
