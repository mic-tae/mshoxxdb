### mshoxxDB - a Versioned Dataset for Electronic Music
This dataset was presented as a [Late Breaking Demo at ISMIR 2024](https://ismir2024program.ismir.net/lbd_423.html) in San Francisco, CA, including the [paper](https://ismir2024program.ismir.net/lbd_423.html#lbd) (as an extended abstract), [poster](https://ismir2024program.ismir.net/lbd_423.html#poster), and [demo video](https://ismir2024program.ismir.net/lbd_423.html#video). It was initially studied in [this EURASIP article](https://asmp-eurasipjournals.springeropen.com/articles/10.1186/s13636-025-00398-2).

### Description
- mshoxxDB version 1.0/1.1 consists of 18 full-length pieces of music in the genre of Electronic Music  
- spans a number of subgenres: Video Game, 8-Bit (Chiptune), EDM, Pop, House, Chillout/Dreamy  
- suitable for a variety of tasks in the field of Music Information Retrieval (MIR), such as Source Separation, Multi-Pitch Estimation, Beat Detection, Tempo Estimation  
- particularly interesting for instrument-agnostic methods and evaluations of model generalization due to wide variety of synthetic and traditional timbres  

### Content Overview
- 18 full-lengths pieces of music, 61 minutes of audio in total
- mixtures and multi-tracks in FLAC format (44.1 kHz, 16-Bit, Mono, compression level 6)
- track-wise MIDI files
- CSV metadata with genre, tempo, time signature, and artist information
- ```ms12``` and ```ms14``` dataset splits, as described in the initial study (see above)

### Technical Notes
Not all mixtures are exact sums of their respective multi-tracks. Some mixtures may contain additional processing in the form of limiters and compression (on the full mix or side-chain compression from one track to another). **_No harmonic effects were added onto the mixtures_** (= effects such as reverbs, echos, and delays that add more harmonic information and would result in mismatches between MIDI and audio).

### License
All contents are distributed under Creative Commons BY-NC-SA 4.0.

### Access & Download
mshoxxDB can be downloaded from **https://doi.org/10.5281/zenodo.13284494**.  
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

### Changes in Version 1.1 (16 July 2025)
- changes all previous file version numbers simply to "v1" for consistency
- includes dataset splits sets ```ms12``` and ```ms14``` (as .json)
- adds README and LICENSE files

### Known Issues in Version 1.1
- typo in folder name "Güte_des_Geschicks_v1": Umlaut "ü" should be "ue" (as referenced in the .json files)

### Future Plans
- 1.2: add segment infos per song
- 2.0: add more songs, and (maybe) make everything available in Stereo
