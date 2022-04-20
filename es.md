Spanish Phoneme set

|   | Type    |
| - | ------- |
| C |Consonant|
| V |Vowel    |
| S |Semivowel|


Phonemes:

| Phoneme       | IPA | X-Sampa | Type | Description          | Example Word | Mexican Example |
| ------------- | --- | ------- | ---- | -------------------- | ------------ | --------------- |
| a             | a   | a       | V    | open fr unrounded    | c*a*sa     |
| e             | e   | e       | V    | cl-mid fr unrounded  | m*e*sa     |
| i             | i   | i       | V    | cl front unrounded   | *i*sla     |
| o             | o   | o       | V    | cl-mid back rounded  | gat*o*     |
| u             | u   | u       | V    | cl back rounded      | *u*no      |
| ------------- |     |         |      |                      |              |
| p             |     |         | C    |                      | *p*ollo      |
| b             |     |         | C    | Hard b               | *b*estia, en*v*idia |
| bv<sup>4</sup>|     |         | C    | Soft b               | be*b*é, vi*v*a |
| t             |     |         | C    |                      | *t*ango      |
| d             |     |         | C    |                      | *d*edo       |
| dj            |     |         | C    |DO NOT LABEL. Allophone for `g` in front of some vowels and is handled contextually. |              |
| k             |     |         | C    |                      | *c*asa, *k*ilo |
| g             |     |         | C    | Hard g               | *g*ato             |
| gh<sup>5</sup>| ɣ   | G       | C    | Soft g               | ami*g*o, do*c*tor |
| s             |     |         | C    | s and z sounds       | *s*al, i*s*la|
| z<sup>10</sup>|     |         | C    |                      | ca**z**ar    |
| ch            | tʃ  |         | C    |                      | *ch*iste     |
| ts<sup>8</sup>| t s |         | C    | upper-class chilean "ch" |               |                 |
| sh<sup>1</sup>| ʃ   |         | C    | REFERENCE ALLOPHONE  |              | e**ch**ador
| zh<sup>2</sup>|     |         | C    | REFERENCE ALLOPHONE  |              |
| f             |     |         | C    |                      | *f*ase       |
| v<sup>7</sup> |     |         | C    | REFERENCE ALLOPHONE. DO NOT USE.  | a*f*gano |
| x<sup>9</sup> |     |         | C    |                      | *j*amón, *g*eneral |
| dh            |     |         | C    |                      | eng: *th*em  |
| n             |     |         | C    |                      | *n*ido, domi*ng*o |
| ny            |     |         | C    |                      | ñ            |
| m             |     |         | C    |                      | *m*esa       |
| w             |     |         | S    |                      | n*u*eve, c*u*anto |
| y<sup>6</sup> |     |         | C+S  |                      | sayo, tierra |
| ll<sup>3</sup>|     |         | C    |palatal lateral approx|              |
| r             |     |         | C    |                      | ca*r*o       |
| rr            |     |         | C    |                      | pe*rr*o      |
| l             |     |         | C    |                      | *l*ino, a*l*tar |

Additional Phonemes:

| Phoneme | Description  | Descripción |
| ------- | ------------ | ----------- |
| br      | Breath       | 
| exh     | Exhale       | 
| axh     | Voiced Exhale|
| pau     | Silence      | 
| sil     | Do not use   | 
| q       | Glottal stop | 
| cl      | closure      |
| vf      | vocal fry    |

<sup>1</sup> Is sometimes (rarely) used as an alterative to `[ll]` and `[y]`. Use `[ll]` instead in cases where `[sh]` is used for "ll".

<sup>2</sup> Use `[ll]` instead. Alternate pronuncation of ll (and sometimes "y") for users from Argentina/The Southern Cone.

<sup>3</sup> Some speakers enounter "yeísmo", or the merging of "ll" and "y". These speakers can label "ll" as `[y]` instead to slightly reduce the amount of training data needed.

<sup>4</sup> Some speakers merge the hard and soft "b" sounds. These speakers can label all "b" as `[b]` and ignore the `[bv]` phoneme. Speakers without this merger can also drop `[bv]` to simplify the dataset, which will cause most "b" will sound soft (due to more isntances of the soft sound in speech). Doing so creates a slight risk that the model may use a hard "b" at an incorrect time.

<sup>5</sup> Some speakers merge the hard and soft "g" sounds. These speakers can label all "g" as `[g]` and ignore the `[gh]` phoneme. Speakers without this merger can also drop `[gh]` to simplify the dataset. Doing so creates a risk that the model may use the incorrect sound.

<sup>6</sup> The `y` phoneme works as both a consonant AND semivowel. This is thanks to NNSVS being able to learn context.

<sup>7</sup> `v` is an allophone of f before voiced consonants. Just use `f` since it's handled contextually.
  
<sup>8</sup> `ts` is used intead of `ch` for upper-class chilean speakers. Please refer to example audio.
For lower-class chilean speakers, `ch` is replaced with `sh`.
NOTE: STILL LABEL AS `ch` FOR DICTIONARY COMPATIBILITY AND USAGE CONSISTENCY. ALSO READ THE EXPLANATION. If a speaker mixes between the two then use both phonemes . But if they almost always replace the sound then follow that guidance.

<sup>9</sup> `x` covers all "h"/"soft J" sounds contextually. So only one phoneme is required. For speakers who want to differenciate, the `h` phoneme could be used along with `x`. `h` being the glottal fricative and `x` being the velar fricative. Note this will increase the amount of data required and won't be supported in the dictionary.

<sup>10</sup> `z` used to be for sounds like the voiced "s" in "isla". However NNSVS handles this contextually and only `s` is needed for both cases. Just use `s` as an ending consonant in a note for proper context. This was changed at some point and now does the lexical "z" sound in words like "cazar" instead of `th`. If you are using an older dataset, you'll need to convert `th` to `z` and `z` to `s`.
