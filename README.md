
## UrbanSound-Spectrogram

This dataset contains spectrogram for 8732 labeled sound excerpts (<=4s) of urban sounds from 10 classes:
*air_conditioner, car_horn, children_playing, dog_bark, drilling, engine_idling, gun_shot, jackhammer, siren, and street_music.*

The sound excerpts are from the *UrbanSound8K dataset*<sup>[1]</sup>. The audio files of urban sounds includes 8732 audio files in WAV format.

### File structure and filename metadata

The filenames for the created spectrograms are same as the corresponding files in UrbanSound8K dataset. The files are pre-sorted into ten folders (folders named fold1-fold10).

The name of the files acts as a metadata and follows this format: **[fsID]-[classID]-[occurrenceID]-[sliceID].wav**, where:

*[fsID]* = the Freesound ID of the recording from which this excerpt (slice) is taken.

*[classID]*<sup>*</sup> = a numeric identifier of the sound class.

*[occurrenceID]* = a numeric identifier to distinguish different occurrences of the sound within the original recording.

*[sliceID]* = a numeric identifier to distinguish different slices taken from the same occurrence.



*The numeric identifier of the sound class *[classID]*:

0 = air_conditioner

1 = car_horn

2 = children_playing

3 = dog_bark

4 = drilling

5 = engine_idling

6 = gun_shot

7 = jackhammer

8 = siren

9 = street_music

### Purpose
The purpose to create this dataset was to help the academicians and researchers working in the domain of sound feature extraction and classification using neural networks.
Creation of the spectrogram or wave-plot is often the prerequisite for the sound classification neural network. Creating these is compute-intensive and time taking. We wanted to provide a better starting point for the students, researchers and academicians with limited resources to directly work on top of the provided spectrograms.

For researchers with limited bandwidth, all the ten folders in the dataset is available as different branches in this repo, so that they can clone only a specific branch and work by using the data available in a single folder as well.

### Usage
 
To use the full dataset:

    git clone https://github.com/mashrin/UrbanSound-Spectrogram.git

To use the data in a specific folder(say fold1):

    git clone -b fold1 --single-branch https://github.com/mashrin/UrbanSound-Spectrogram.git

### Upcoming

 - The package to create the spectrogram.
 - Sample sound classification neural network using these spectrogram.
 - Spectrogram creation for other well-known audio dataset.
 
### Contributors

Mashrin Srivastava

Saumya Suvarna

This work was done a couple of years back for our Graphics and Multimedia course project at VIT University.

### Reference:
[1] https://urbansounddataset.weebly.com/
