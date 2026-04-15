[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.15881577.svg)](https://doi.org/10.5281/zenodo.15881577)

### mshoxxDB - a Versioned Dataset for Electronic Music
This dataset was presented as a [Late Breaking Demo at ISMIR 2024](https://ismir2024program.ismir.net/lbd_423.html) in San Francisco, CA, including the [paper](https://ismir2024program.ismir.net/lbd_423.html#lbd) (as an extended abstract), [poster](https://ismir2024program.ismir.net/lbd_423.html#poster), and [demo video](https://ismir2024program.ismir.net/lbd_423.html#video). It was initially studied in [this EURASIP article](https://asmp-eurasipjournals.springeropen.com/articles/10.1186/s13636-025-00398-2).  

### Description
- mshoxxDB consists of 18 full-length pieces of music, 61 minutes of audio in total  
- covers subgenres: Video Game, 8-Bit (Chiptune), EDM, Pop, House, Chillout/Dreamy styles  
- supports tasks in the field of Music Information Retrieval (MIR) such as source separation, multi-pitch estimation, beat detection, tempo estimation  
- particularly well suited for instrument-agnostic methods and model generalization evaluations due to diverse synthetic and traditional timbres  
- created by Michael Taenzer in Reason Studios DAW  

### Content Overview
- 18 full-length pieces of music, 61 minutes of audio in total  
- mixtures and multitrack stems in FLAC format (44.1 kHz, 16-bit, mono, compression level 6)  
- track-level MIDI files  
- CSV metadata including genre, tempo, time signature, and artist information  
- ```ms12``` and ```ms14``` dataset splits in JSON format, as described in the initial study (see above)  

### Technical Notes
Not all mixtures are exact sums of their respective multi-tracks. Some mixtures may contain additional processing in the form of limiters and compression, e.g. applied to the full mix or through side-chain compression between tracks.
No harmonic effects were added onto the mixtures, such as reverb, echo, or delay, as these would introduce additional harmonic content, resulting in mismatches between MIDI and audio.  

### License
All contents are distributed under Creative Commons BY-NC-SA 4.0.

### Access & Download & Demo
mshoxxDB can be downloaded from **https://doi.org/10.5281/zenodo.13284494**. Zenodo hosts the canonical archived release of mshoxxDB.  
For a few listening examples, please visit this repo's GitHub Pages at **https://mic-tae.github.io/mshoxxdb/**.

### Citation
Should you use this dataset in your work, please cite it as follows (bibtex):
```
@misc {taenzer:mshoxxDB:2024,
  author    = {Taenzer, Michael},
  title     = {{mshoxxDB - a Versioned Dataset for Electronic Music}},
  booktitle = {{Late-Breaking and Demo Session of the 25th International Conference on Music Information Retrieval (ISMIR)}},
  address   = {{San Francisco, CA, USA}},
  year      = {2024},
}
```
### Future versions
Future versions of mshoxxDB may include additional music, segmentation annotations for each piece, and possibly stereo audio data.  

### Community
Contributions to this dataset are welcome in all forms, e.g. by adding new music, annotations, or other suggestions that could help improve mshoxxDB.  

### Changes in Version 1.1
- changes all previous file version numbers simply to "v1" for consistency  
- adds ```ms12``` and ```ms14``` dataset splits (JSON files)  
- adds a LICENSE file, and a README file  

### Known Issues in Version 1.1
- typo in folder name "Güte_des_Geschicks_v1": Umlaut "ü" should be "ue" (as referenced in the .json files)  
