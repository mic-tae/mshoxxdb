### Changelog
Version 1.2 (15 April 2026)  
- added "metadata.csv" back into the archive  
- substantially restructured "metadata.csv":  
  - new columns: "piece_id", "artist", "bpm_min", "bpm_max"  
  - renamed columns: "genre" -> "genres", "length" -> "duration_seconds", "timesig" -> "time_signature"  
  - dropped column: "tempo"  
- json files now use "piece_id" instead of filenames as identifier  
- changed all remaining umlauts "ü" -> "ue"
- substantially extended "README.txt"
- small changes to "LICENSE.txt"
  
Version 1.1 (16 July 2025)  
- renamed all files to reflect main DB version number v1  
- changed umlaut "ü" from "Güte" -> "Guete"  
- added dataset splits "ms12" (1 json) and "ms14" (3 jsons) as described and used [here](https://doi.org/10.1186/s13636-025-00398-2)  
- added "README.txt"
- added "LICENSE.txt"

Version 1 (14 November 2024)  
- Initial release
