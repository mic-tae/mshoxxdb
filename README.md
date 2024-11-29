### mshoxxDB - a Versioned Dataset for Electronic Music

This dataset was presented as a [Late Breaking Demo at ISMIR 2024](https://ismir2024program.ismir.net/lbd_423.html) in San Francisco, CA, including the [paper](https://ismir2024program.ismir.net/lbd_423.html#lbd) (as an extended abstract), [poster](https://ismir2024program.ismir.net/lbd_423.html#poster), and [demo video](https://ismir2024program.ismir.net/lbd_423.html#video).

### Description

Version 1 of mshoxxDB consists of 18 full-length pieces of music in the genre of Electronic Music, totaling 61 minutes of audio.
The dataset spans a number of sub-genres of Electronic Music: Video Game, 8-Bit (Chiptune), EDM, Pop, House, Chillout/Dreamy.
The dataset suits itself for a variety of tasks in the field of Music Information Retrieval (MIR), such as Source Separation, Multi-Pitch Estimation, Beat Detection, Tempo Estimation.
It is particularly interesting for instrument-agnostic methods and evaluations of model generalization due to wide variety of synthetic and traditional timbres.

mshoxxDB contains:
- mixtures and multi-tracks in FLAC format (44.1 kHz, 16-Bit, Mono, compression level 6)
- track-wise MIDI files
- CSV metadata with genre, tempo, time signature, and artist information

### Technical Properties

Not all mixtures are exact sums of their respective multi-tracks. Depending on the piece, the mixtures may contain additional processing in the form of compression (on the full mix or side-chain compression from one track to another), and limiters. **_No harmonic effects are added onto the mixtures_** (= effects that add harmonic information (reverbs, echos, delays) resulting in mismatches between MIDI and audio).

### License
All contents are distributed under Creative Commons BY-NC-SA 4.0.

### Access & Download
mshoxxDB can be downloaded from **https://doi.org/10.5281/zenodo.13284495**.

### Demo Page
For a few listening examples, please visit this repo's github page at **https://mic-tae.github.io/mshoxxdb/**.

### Upcoming changes
- make dataset available in Stereo
