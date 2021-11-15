# Digit match

Simple scripts to read pairs of digits from a .mp4 file and output the data as a .csv.

## Getting Started

### Dependencies

* Needs Python 3 and ```opencv``` installed.

### Preparing digits

The included digits should work for ```picamera``` annotations.
If these digits aren't working, the ```make_digits.py``` script can take an image and extract 2 digits (provided the coordinates are changed).
To make a pair of digits run the following:
```
python3 make_digits.py -i PATH_TO_IMAGE -o NAME_FIRST_DIGIT -t NAME_SECOND_DIGIT
```

### Executing program
* To read digits from a video file run the following:
```
python3 get_temp.py -v PATH_TO_VIDEO -d PATH_TO_DIGIT_DIRECTORY/
```
Alternatively, the script can also find all the .mp4 files in a directory and read digits for all of them:
```
python3 get_temp.py -v PATH_TO_VIDEO_DIRECTORY/ -d PATH_TO_DIGIT_DIRECTORY/
```

## Authors

* Mário Artur Mira


## Version History

* 0.1
    * Initial Release
