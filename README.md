# General Tensorflow Image Classifier



## Requirements

* [docker](https://www.docker.com/)

## Usage 

A "classifier" directory with a directory "data" inside it with all the images.
For example
```
 [any_path]/the_classifier/
 [any_path]/the_classifier/data
 [any_path]/the_classifier/data/ant_newman
```
Here you put your images, so if we are making an Ant Newman classifier, it would be photoraphs of me throughout the bearded and non-bearded ages.

This directory has the samples and the trained classifier after execution of "train.sh". 

## Train process
 
In your docker environment:
```
 ./train.sh [any_path]/the_classifier
``` 
## Guess process

For a single guess:
```
 ./guess.sh [any_path]/the_classifier /yourfile.jpg
```

To guess an entire directory
```
./guessDir.sh [any_path]/classifier [any_path]/srcDir [any_path]/destDir
``````

Requires an absolute file path for classifier and images because the script dos not support relative path (volume mounting)

# Credits

Thanks to [Xblaster](https://github.com/xblaster) 