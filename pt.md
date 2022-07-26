### NOTICE
By using all OR ANY PART of this project you MUST follow our license at https://github.com/DYVAUX/nnsvs-english-support/blob/main/LICENSE.md
This includes using parts of our work in yours. If you have questions about the license please contact us.
We should not have to include this notice in our files but bad actors had forced our hand.
___

Phoneme reference for Portuguese (EU)

## Other:

| Phoneme | X-SAMPA | Description |
| ------- | ------- | ----------- |
| br      |         | Inhale      |
| exh     |         | Exhale      |
| axh     |         | Voiced Exhale|
| pau     |         | Silence     |
| q       | ?       | Glottal Stop|
| cl      |         | Closure (Held Consonants) |
| vf      |         | Vocal Fry   |
| trash   |         | Junk Phoneme| 

## Vowels:
| Phoneme | X-SAMPA | Explaination                    | Example                                 |
|---------|---------|---------------------------------|-----------------------------------------|
| a       | a       | central-open unrounded vowel    | d<ins><b>á</ins></b>                    |
| ao      | O Q     | open-mid back rounded vowel     | form<ins><b>o</ins></b>sa               |
| au      | 6       | near-open central vowel         | c<ins><b>â</ins></b>mera                |
| e       | e       | close-mid front unrounded vowel | s<ins><b>ê</ins></b>                    |
| eh      | E       | open-mid front unrounded vowel  | m<ins><b>e</ins></b>ta                  |
| i       | i       | close-front unrounded vowel     | s<ins><b>i</ins></b>                    |
| o       | o       | close-mid back rounded vowel    | av<ins><b>ô</ins></b>                   |
| u       | u       | close-back rounded vowel        | r<ins><b>u</ins></b>     a              |
| uu      | M       | close-back unrounded vowel      | p<ins><b>e</ins></b>gar, jur<ins><b>e</ins></b> |

## Nasal-Vowels:
| Phoneme | X-SAMPA | Explaination                    | Example                                 |
|---------|---------|---------------------------------|-----------------------------------------|
| an      | 6~      |                                 | canto             |
| en      | e~      |                                 | entro             |
| in      | i~      |                                 | vim             |
| on      | o~      |                                 | sombra             |
| un      | u~      |                                 | mundo             |

## Semi-Vowels:
(Semi-vowels function as consonants and perform "diphthong-like" tasks.)
| Phoneme | X-SAMPA | Explaination                    | Example                                 |
|---------|---------|---------------------------------|-----------------------------------------|
| y       | j       | palatal approximant             | dois |
| w       | w       | labial-velar approximant        | ouro                                   |

## Consonants:
| Phoneme | X-SAMPA | Explanation                        | Example                   |
|---------|---------|------------------------------------|---------------------------|
| b       | b       | voiced bilabial plosive            |                           |
| bh      | B       | voiced bilabial fricative          |                           |
| ch      | tS      | voiceless postalveolar affricate   |                           |
| d       | d       | voiced alveolar plosive            |                           |
| dh      | D       | voiced dental fricative            |                           |
| f       | f       | voiceless labiodental fricative    |                           |
| g       | g       | voiced velar plosive               |                           |
| gh      | G       | voiced velar fricative             |                           |
| k       | k       | voiceless velar plosive            |                           |
| l       | l       | lateral alveolar approximant       |                           |
| lh (*)  | L       | voiced palatal lateral approximant |                           |
| m       | m       | bilabial nasal                     |                           |
| n       | n       | alveolar nasal                     |                           |
| nh      | J       | palatal nasal                      |                           |
| p       | p       | voiceless bilabial plosive         |                           |
| r       | 4       | alveolar flap                      |                           |
| rh      | R       | voiced uvular fricative            |                           |
| s       | s       | voiceless alveolar fricative       |                           |
| sh      | S       | voiceless postalveolar fricative   |                           |
| t       | t       | voiceless alveolar plosive         |                           |
| z       | z       | voiced alveolar fricative          |                           |
| zh      | Z       | voiced postalveolar fricative      |                           |
| v       | v       | voiced labiodental fricative       |                           |

## Dialect Allophones:
These will <ins><b>never</ins></b> be used in a dataset.
| Phoneme | X-SAMPA | Explanation                           | Example               | Dialect                                               |
|---------|---------|---------------------------------------|-----------------------|-------------------------------------------------------|
| ng      | N       | velar nasal                           |                       | Reference allophone for n (before velar consonants).  |


* [lh] is dropped for many speakers. Label as [j] instead.
