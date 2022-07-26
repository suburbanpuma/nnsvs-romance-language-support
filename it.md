### NOTICE
By using all OR ANY PART of this project you MUST follow our license at https://github.com/DYVAUX/nnsvs-english-support/blob/main/LICENSE.md
This includes using parts of our work in yours. If you have questions about the license please contact us.
We should not have to include this notice in our files but bad actors had forced our hand.
___

Italian Phoneme set

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
| axh     |         | Voiced Exhale|
| pau     |         | Silence     |
| q       | ?       | Glottal Stop|
| cl      |         | Closure (Held Consonants) |
| vf      |         | Vocal Fry   |
| trash   |         | Junk Phoneme| 


## Vowels:
| Phoneme       | X-Sampa | Description          | Example      | 
| ------------- | ------- | -------------------- | ------------ |
| a             | a       | open fr unrounded    | *a*lto       |
| e             | e       | cl-mid fr unrounded  |              |
| i             | i       | cl front unrounded   |              |
| o             | o       | cl-mid back rounded  |              |
| u             | u       | cl back rounded      |              |
| eh            | E       | op-mid-fr unrounded  |              |
| ao            | O       | op-mid-back rounded  |              |

## Consonants:
| Phoneme       | X-Sampa | Description          | Example      | 
| ------------- | ------- | -------------------- | ------------ |
| p             |         |                      |              |
| b             |         |                      |              |
| ts<sup>1</sup>|         |                      | mar*z*o      |
| t             |         |                      |              |
| d             |         |                      |              |
| dg            |         |                      | gelo, magia  |
| k             |         |                      |              |
| g             |         |                      |              |
| s             |         |                      |              |
| z             |         |                      |              |
| zz            |         |                      | mezzo        |
| ch            | tS      |                      | certo        |
| sh            | S       |                      |              |
| zh            | Z       | foreign addition     |              |
| f             |         |                      |              |
| v             |         |                      |              |
| h             |         | foreign addition     |              |
| th            |         | foreign addition     |              |
| n             |         |                      | punto, anfibio |
| gn            |         |                      | bagno, gnocchi |
| m             |         |                      | mano         |
| w             |         |                      |              |
| j             |         |                      |              |
| gl            |         |                      | glielo       |
| r             |         |                      |              |
| l             |         |                      |              |

## Dialect Allophones:
These will <ins><b>never</ins></b> be used in a dataset.
| Phoneme | X-SAMPA | Explanation                           | Example               | Dialect                                               |
|---------|---------|---------------------------------------|-----------------------|-------------------------------------------------------|
| ng      | N       | velar nasal                           |                       | Reference allophone for n (before velar consonants).  |


<sup>1</sup> It is possible to label as `[t][s]` instead of a unique phoneme
