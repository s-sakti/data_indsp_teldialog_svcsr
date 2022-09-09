# INDspeech02: INDspeech_TELDIALOG_SVCSR

This is the first Indonesian speech dataset for small vocabulary continuous speech recognition (SVCSR). The data was developed by TELKOMRisTI (R&D Division, PT Telekomunikasi Indonesia) in collaboration with [Advanced Telecommunication Research Institute International (ATR) Japan](https://www.atr.jp/) and Bandung Institute of Technology (ITB) under the Asia-Pacific Telecommunity (APT) project in 2004 [[Sakti et al., 2004](https://www.isca-speech.org/archive_v0/interspeech_2004/i04_1037.html)]. Although it was originally developed for a telecommunication system for hearing and speaking impaired people, it can be used for other applications, i.e., automatic call centers. Furthermore, as all speakers utter the same sentences, it can also be used for voice conversion tasks. 

## Text and Speech Resources

The text is based on a word vocabulary which is derived from some necessary dialog calls, such as dialog calls with the 119 emergency department, 108 telephone information department, and ticket reservation department. In total, it consists of 20,000 utterances (about 18 hours of speech) from the 70-word dialog vocabulary of 100 sentences (including single word sentences) each uttered by 200 speakers (100 Females, 100 Males). The age is limited to middle age (20-40 years), but they present a wide range of spoken dialects from different ethnic groups.

Table. The percentage of population according to 2000 Census (%A) vs the percentage distribution of speakers in the corpus (%B). 

| Island     |  %A |  %B | Native Languages                         |
| ---------- | --- | --- | ---------------------------------------- |
| Java       | 60% | 67% | Sundanese,Javanese, Madurese, Indonesian |
| Sumatra    | 21% | 21% | Acehnese,Lampung Batak, Minang, Malays   | 
| Sulawesi   |  7% |  5% | Makassar,Minahasa, Bugis, Gorontalo      | 
| Kalimantan |  5% |  2% | Banjar                                   |
| Others     |  7% |  5% | Balinese, Ambonese, Tionghoa             |


The recording is conducted in parallel for both clean and telephone speech, but we open only the clean speech due to quality issues on telephone speech. Each audio file is a single-channel 16-bit PCM WAV with a sample rate of 16000 Hz. These utterances are equally split into training and test sets with 100 speakers (50 Females, 50 Males) in each set.

## File Format

```
"FHJ_U097.wav" 
```

- Gender ID: F or M
- Speaker ID: XX
- Utterance ID: UXXX (001-100) 

## License

This data is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/) International License (see LICENSE_CC-BY-NC-4.0.txt). You can use the data free for non-commercial purposes, but you have to cite our paper if your work uses our data in your publication. If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original. Furthermore, you are not allowed to create a copy of this dataset and share it publicly in your own repository without our permission.

## Citation

Please cite the following paper [[Sakti et al, 2004](https://www.isca-speech.org/archive_v0/interspeech_2004/i04_1037.html)]:

```
@inproceedings{sakti-icslp-2004,
    title = "Indonesian Speech Recognition for Hearing and Speaking Impaired People",
    author = "Sakti, Sakriani and Hutagaol, Paulus and Arman, Arry Akhmad and Nakamura, Satoshi",
    booktitle = "Proc. International Conference on Spoken Language Processing (INTERSPEECH - ICSLP)",
    year = "2004",
    pages = "1037--1040"
    address = "Jeju Island, Korea"
}
```
