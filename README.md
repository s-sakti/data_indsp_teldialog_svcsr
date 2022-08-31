# data_indsp_teldialog_svcsr

# INDspeech_DIGIT_CDSR

This is one of the first Indonesian speech datasets for connected digit speech recognition (CDSR). The data was developed by TELKOMRisTI (R&D Division, PT Telekomunikasi Indonesia) under the Asia-Pacific Telecommunity (APT) project. Although it was originally developed for a telecommunication system for hearing and speaking impaired people, it can be used for other applications, i.e., automatic call centers that recognize telephone numbers. 

## Text and Speech Resources

The text consists of connected digit tasks among the following digit words: 1 (satu), 2 (dua), 3 (tiga), 4 (empat), 5 (lima), 6 (enam), 7 (tujuh), 8 (delapan), 9 (sembilan), 0 (nol and kosong). It is an adaptation of the official [English AURORA2 dataset](http://aurora.hsnr.de/aurora-2.html) for [noisy digit speech recognition tasks](http://dnt.kr.hsnr.de/aurora/download/asr2000_final_footer.pdf), which is also related to the Japanese version [AURORA2J](http://research.nii.ac.jp/src/en/CENSREC-1.html). So if you have these AURORA2 and AURORA2J, you will have an English-Japanese-Indonesian parallel dataset. [The parallel English-Japanese dataset with digit-emphasized version](http://www.phontron.com/pcbeu/) is also available. 

The recording is conducted in parallel for both clean and telephone speech, but we open only the clean speech due to quality issues on telephone speech. Each audio file is a single-channel 16-bit PCM WAV with a sample rate of 16000 Hz. The speech is recorded with 214 speakers (20-40 years). Both genders are distributed evenly. The age is limited to middle age (20-40 years), but they present a wide range of spoken dialects from different ethnic groups.

Table. The percentage of population according to 2000 Census (%A) vs the percentage distribution of speakers in the corpus (%B). 

| Island     |  %A |  %B | Native Languages                         |
| ---------- | --- | --- | ---------------------------------------- |
| Java       | 60% | 67% | Sundanese,Javanese, Madurese, Indonesian |
| Sumatra    | 21% | 21% | Acehnese,Lampung Batak, Minang, Malays   | 
| Sulawesi   |  7% |  5% | Makassar,Minahasa, Bugis, Gorontalo      | 
| Kalimantan |  5% |  2% | Banjar                                   |
| Others     |  7% |  5% | Balinese, Ambonese, Tionghoa             |

## Training and Test Dataset

As it is close to the official AURORA2 digit task, The data consists of 8440 training utterances (spoken by 55 Females, 55 Males) and 4004 testing utterances (spoken by 52 Females, 52 Males), which are equally split into four subsets (1001 utterances in each). These training and testing sets consist of about 8 and 4 hours of speech, respectively.

## File Format

```
"FSK_K281KA.{wav,txt}" 
```

- Gender ID: F or M
- Speaker ID: XX
- Sentence: K281K = "Kosong Dua Delapan Satu Kosong"
- ".wav" for speech and ".txt" for transcription

## License

This data is licensed under the Creative Commons Attribution-NonCommercial 4.0 (CC BY-NC 4.0) International License (see LICENSE_CC-BY-NC-4.0.txt).
You can use the data free for non-commercial purposes, but you have to cite our paper if your work uses our data in your publication. Furthermore, you are not allowed to create a copy of this dataset and share it publicly in your own repository without our permission.
Citation

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
