### mshoxxDB - a Versioned Dataset for Electronic Music
This dataset was presented as a [Late Breaking Demo at ISMIR 2024](https://ismir2024program.ismir.net/lbd_423.html) in San Francisco, CA, including the [paper](https://ismir2024program.ismir.net/lbd_423.html#lbd) (as an extended abstract), [poster](https://ismir2024program.ismir.net/lbd_423.html#poster), and [demo video](https://ismir2024program.ismir.net/lbd_423.html#video).
It was initially studied in [this EURASIP article](https://asmp-eurasipjournals.springeropen.com/articles/10.1186/s13636-025-00398-2).

### Description
Version 1.1 of mshoxxDB consists of 18 full-length pieces of music in the genre of Electronic Music, totaling 61 minutes of audio.
The dataset spans a number of subgenres of Electronic Music: Video Game, 8-Bit (Chiptune), EDM, Pop, House, Chillout/Dreamy.  
The dataset is suitable for a variety of tasks in the field of Music Information Retrieval (MIR), such as Source Separation, Multi-Pitch Estimation, Beat Detection, Tempo Estimation.
It is particularly interesting for instrument-agnostic methods and evaluations of model generalization due to wide variety of synthetic and traditional timbres.

mshoxxDB contains:
- mixtures and multi-tracks in FLAC format (44.1 kHz, 16-Bit, Mono, compression level 6)
- track-wise MIDI files
- CSV metadata with genre, tempo, time signature, and artist information
- ms12 and ms14 dataset splits, as described in the initial study (see above)

### Technical Properties
Not all mixtures are exact sums of their respective multi-tracks. The mixtures may contain additional processing in the form of limiters and compression (on the full mix or side-chain compression from one track to another). **_No harmonic effects were added onto the mixtures_** (= effects such as reverbs, echos, and delays that add more harmonic information and would result in mismatches between MIDI and audio).

### License
All contents are distributed under Creative Commons BY-NC-SA 4.0.

### Access & Download
mshoxxDB can be downloaded from **https://doi.org/10.5281/zenodo.13284494**.

### Demo Page
For a few listening examples, please visit this repo's github page at **https://mic-tae.github.io/mshoxxdb/**.

### Citation
Should you use this dataset in your work, please cite it the following way (bibtex):
```
@misc {taenzer:mshoxxDB:2024,
  author    = {Taenzer, Michael},
  title     = {{mshoxxDB - a Versioned Dataset for Electronic Music}},
  booktitle = {{Late-Breaking and Demo Session of the 25th International Conference on Music Information Retrieval (ISMIR)}},
  address   = {{San Francisco, CA, USA}},
  year      = {2024},
}
```

### Changes in Version 1.1
This version was released on 16 July 2025.
- changes all file version numbers simply to v1 (as this is the first release)
- includes dataset splits sets ```ms12``` and ```ms14```
- adds README and LICENSE files

### Upcoming changes
- 2.0: (maybe) make dataset available in Stereo
