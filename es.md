Spanish Phoneme set

Phonemes:

| Phoneme       | IPA | X-Sampa | Type | Description          | Example Word | Mexican Example |
| ------------- | --- | ------- | ---- | -------------------- | ------------ | --------------- |
| a             | a   | a       | V    | open fr unrounded    | c*a*sa     |
| e             | e   | e       | V    | cl-mid fr unrounded  | m*e*sa     |
| i             | i   | i       | V    | cl front unrounded   | *i*sla     |
| o             | o   | o       | V    | cl-mid back rounded  | gat*o*     |
| u             | u   | u       | V    | cl back rounded      | *u*no      |
| ------------- |     |         |      |                      |              |
| p             |     |         | C    |                      |              |
| b             |     |         | C    | Hard b               |              |
| bv<sup>4</sup>|     |         | C    | Soft b               |              |
| t             |     |         | C    |                      |              |
| d             |     |         | C    |                      |              |
| dj            |     |         | C    |                      |              |
| k             |     |         | C    |                      |              |
| g             |     |         | C    | Hard g               |              |
| gh<sup>5</sup>| ɣ   | G       | C    | Soft g               |              |
| s             |     |         | C    |                      |              |
| z             |     |         | C    |                      |              |
| ch            |     |         | C    |                      |              |
| sh<sup>1</sup>|     |         | C    |                      |              | e**ch**ador
| zh<sup>2</sup>|     |         |      |                      |              |
| f             |     |         | C    |                      |              |
| v             |     |         | C    |                      |              |
| x             |     |         | C    |                      |              |
| th            |     |         | C    |                      |              |
| dh            |     |         | C    |                      |              |
| n             |     |         | C    |                      |              |
| ny            |     |         | C    |                      |              |
| m             |     |         | C    |                      |              |
| w             |     |         | S    |                      | nueve        |
| y             |     |         | C    |                      |              |
| ll<sup>3</sup>|     |         | C    | palatal lateral approx |              |
| r             |     |         | C    |                      |              |
| rr            |     |         | C    |                      |              |
| l             |     |         | C    |                      |              |

Additional Phonemes:

| Phoneme | Description  | Descripción |
| ------- | ------------ | ----------- |
| br      | Breath       | 
| exh     | Exhale       | 
| axh     | Voiced Exhale|
| pau     | Silence      | 
| sil     | Do not use   | 
| q       | Glottal stop | 

<sup>1</sup> Is sometimes (rarely) used as an alterative to `[ll]`. Use `[ll]` instead in that case.

<sup>2</sup> Use `[ll]` instead. Alternate pronuncation of ll for users from Argentina/The Southern Cone.

<sup>3</sup> Some speakers enounter "yeísmo", or the merging of "ll" and "y". These speakers can label "ll" as `[y]` instead to slightly reduce the amount of training data needed.

<sup>4</sup> Some speakers merge the hard and soft "b" sounds. These speakers can label all "b" as `[b]` and ignore the `[bv]` phoneme. Speakers without this merger can also drop `[bv]` to simplify the dataset, which will cause most "b" will sound soft (due to more isntances of the soft sound in speech). Doing so creates a slight risk that the model may use a hard "b" at an incorrect time.

<sup>5</sup> Some speakers merge the hard and soft "g" sounds. These speakers can label all "g" as `[g]` and ignore the `[gh]` phoneme. Speakers without this merger can also drop `[gh]` to simplify the dataset. Doing so creates a risk that the model may use the incorrect sound.
