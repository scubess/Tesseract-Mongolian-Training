# Tesseract Mongolian Training
This repo provides mongolian cyrillic traineddata built from source using, 
* Tesseract 3.03-rc1 ([Homepage](https://www.google.com))
* Leptonica 1.71 ([Homepage](http://www.leptonica.com/))

## Purpose
The purpose of spending time and efforts in training mongolian cyrillic in Tesseract v3.03 is to use it in iOS 11 and xcode9. And also, to avoid crashes with wierd error in the iOS11, due to mismatch between traineddata and tesseract engine
> actual_tessdata_num_entries_ <= TESSDATA_NUM_ENTRIES:Error:Assert failed:in file ../../ccutil/tessdatamanager.cpp, line 53

NOTE: It doesn't mean that mon.traineddata is trained to work for iOS only. It will work  with tesseract engine v3.03 and above. 

## Training Tesseract
To make it working on iOS11, I ran through the whole training process using the tools provided to train Tesseract 3.03–3.05 for a new language in ubuntu 16.04. Please refer to [Training Tesseract](https://github.com/tesseract-ocr/tesseract/wiki/Training-Tesseract#introduction) github section. 
> How to use the tools provided to train Tesseract 3.03–3.05 for a new language.

## Known Limitations
* No LSTM Training 
* Use mongolian cyrillic text provided by [khangaikh](https://github.com/khangaikh/tesseract-mon)
