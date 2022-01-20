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
| s             |     |         | C    |                      | *s*al        |
| z             |     |         | C    |                      | i*s*la       |
| ch            |     |         | C    |                      | *ch*iste     |
| sh<sup>1</sup>|     |         | C    | REFERENCE ALLOPHONE  |              | e**ch**ador
| zh<sup>2</sup>|     |         | C    | REFERENCE ALLOPHONE  |              |
| f             |     |         | C    |                      | *f*ase       |
| v<sup>7</sup> |     |         | C    | REFERENCE ALLOPHONE. DO NOT USE.  | a*f*gano |
| x             |     |         | C    |                      | *j*amón, *g*eneral |
| th            |     |         | C    |                      | eng: ba*th*  |
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

<sup>1</sup> Is sometimes (rarely) used as an alterative to `[ll]` and `[y]`. Use `[ll]` instead in cases where `[sh]` is used for "ll".

<sup>2</sup> Use `[ll]` instead. Alternate pronuncation of ll (and sometimes "y") for users from Argentina/The Southern Cone.

<sup>3</sup> Some speakers enounter "yeísmo", or the merging of "ll" and "y". These speakers can label "ll" as `[y]` instead to slightly reduce the amount of training data needed.

<sup>4</sup> Some speakers merge the hard and soft "b" sounds. These speakers can label all "b" as `[b]` and ignore the `[bv]` phoneme. Speakers without this merger can also drop `[bv]` to simplify the dataset, which will cause most "b" will sound soft (due to more isntances of the soft sound in speech). Doing so creates a slight risk that the model may use a hard "b" at an incorrect time.

<sup>5</sup> Some speakers merge the hard and soft "g" sounds. These speakers can label all "g" as `[g]` and ignore the `[gh]` phoneme. Speakers without this merger can also drop `[gh]` to simplify the dataset. Doing so creates a risk that the model may use the incorrect sound.

<sup>6</sup> The `y` phoneme works as both a consonant AND semivowel. This is thanks to NNSVS being able to learn context.

<sup>7</sup> `v` is an allophone of f before voiced consonants. Just use `f` since it's handled contextually.
