[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.13284494.svg)](https://doi.org/10.5281/zenodo.13284494)

### mshoxxDB - a Versioned Dataset for Electronic Music
This dataset was presented as a [Late Breaking Demo at ISMIR 2024](https://ismir2024program.ismir.net/lbd_423.html) in San Francisco, CA, including the [paper](https://ismir2024program.ismir.net/lbd_423.html#lbd) (as an extended abstract), [poster](https://ismir2024program.ismir.net/lbd_423.html#poster), and [demo video](https://ismir2024program.ismir.net/lbd_423.html#video). It was initially studied in [this EURASIP article](https://asmp-eurasipjournals.springeropen.com/articles/10.1186/s13636-025-00398-2). More details (Methodology, Getting Started, etc.) available in the archive on Zenodo.

### Description
- mshoxxDB consists of 18 full-length pieces of Electronic Music, 61 minutes of audio in total  
- covers subgenres: Video Game, 8-Bit (Chiptune), EDM, Pop, House, Chillout/Dreamy styles  
- supports tasks in Music Information Retrieval (MIR) such as instrument detection, source separation, multi-pitch estimation, beat detection, tempo estimation  
- particularly well suited for instrument-agnostic methods and model generalization evaluations due to diverse synthetic and traditional timbres  
- created by Michael Taenzer in Reason Studios DAW  

### Content Overview
- 18 full-length pieces of music, 61 minutes of audio in total  
- mixtures and multitrack stems in FLAC format (44.1 kHz, 16-bit, mono, compression level 6)  
- track-level MIDI files  
- CSV metadata including, among others: genres, tempo (bpm), time signature, original composer and artist information  
- ```ms12``` and ```ms14``` dataset splits in JSON format, as described in the initial study (see above)  

### Technical Notes
Not all mixtures are exact sums of their respective multi-tracks. Some mixtures may contain additional processing in the form of limiters and compression, e.g. applied to the full mix or through side-chain compression between tracks. No harmonic effects were added onto the mixtures, such as reverb, echo, or delay, as these would introduce additional harmonic content and could result in mismatches between MIDI and audio.  

### License
All contents are distributed under Creative Commons BY-NC-SA 4.0.

### Access & Download & Demo
mshoxxDB can be downloaded from **https://doi.org/10.5281/zenodo.13284494**. Zenodo hosts the canonical archived release of mshoxxDB.  
For a few listening examples, please visit this repo's GitHub Pages at **https://mic-tae.github.io/mshoxxdb/**.

### Future versions
Future versions of mshoxxDB may include additional music, segmentation annotations for each piece, and possibly stereo audio data.  

### Community
Contributions to this dataset are welcome in all forms, e.g. by adding new music, annotations, or other suggestions that could help improve mshoxxDB.  

### Changelog
Version 1.2 (15 April 2026)  
- added "metadata.csv" back into the archive  
- substantially restructured "metadata.csv":  
  - new columns: "piece_id", "artist", "bpm_min", "bpm_max"  
  - renamed columns: "genre" -> "genres", "length" -> "duration_seconds", "timesig" -> "time_signature"  
  - dropped column: "tempo"  
- json files now use "piece_id" instead of filenames as identifier  
- changed all remaining umlauts "ü" -> "ue"  
- substantially extended this README file  
  
Version 1.1 (16 July 2025)  
- renamed all files to reflect main DB version number v1  
- changed umlaut "ü" from "Güte" -> "Guete"  
- added dataset splits "ms12" (1 json) and "ms14" (3 jsons) as described and used [here](https://doi.org/10.1186/s13636-025-00398-2)  
- added LICENSE file  
- added README file  

Version 1 (14 November 2024)  
- Initial release  
