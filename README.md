# Spotify Data Analysis

## Dataset

- Dataset details - https://www.aicrowd.com/challenges/spotify-million-playlist-dataset-challenge
- Dataset - https://www.aicrowd.com/challenges/spotify-million-playlist-dataset-challenge/dataset_files

|                   | Compressed (zip) | Uncompressed | No. of playlists | Total rows | Total unique tracks | Link |
| ----------------- | ---------------- | ------------ | ---------------- | ---------- | ------------------- | ---- |
| Challenge dataset | 113.3 MB         | 332.2 MB     | 10k              | 281k       | 66k                 | [spotify_million_playlist_dataset_challenge.zip](https://www.aicrowd.com/challenges/spotify-million-playlist-dataset-challenge/dataset_files?unique_download_uri=739&challenge_id=277) |
| Full dataset      | 5.79 GB          | 33.54 GB     | 1 million        | 66 million | 23 million          | [spotify_million_playlist_dataset.zip](https://www.aicrowd.com/challenges/spotify-million-playlist-dataset-challenge/dataset_files?unique_download_uri=738&challenge_id=277) |

## Time taken

|                                                                                                    | Time taken with 10k playlists | Time taken with 1M playlists |
| -------------------------------------------------------------------------------------------------- | ----------------------------- | ---------------------------- |
| **Exploratory Analysis**                                                                           |                               |                              |
| Most popular song                                                                                  | 6.93 s                        | 11min 8s                     |
| Most popular album                                                                                 | 3.15 s                        | 10min 23s                    |
| Most popular artist                                                                                | 2.6 s                         | 9min 50s                     |
| Average playlist duration                                                                          | 2.91 s                        | 9min 4s                      |
| Playlist duration histogram                                                                        | 3.46 s                        | 9min 34s                     |
| Average number of tracks per playlist                                                              | 3.56 s                        | 10min 19s                    |
| Playlist track count histogram                                                                     | ​​3.16 s                        | 10min 37s                    |
| Average number of albums per playlist                                                              | 2.32 s                        | 9min 43s                     |
| Playlist album count histogram                                                                     | 2.47 s                        | 10min                        |
| Most popular song at playlist position 1, 2 and 3                                                  | 6.08 s                        | 27min 46s                    |
| Top 5 most followed playlists                                                                      | 1.7 s                         | 9min 18s                     |
| Correlation between number of followers and whether most popular song is present in that playlist  | 4.15 s                        | 18min 43s                    |
| Correlation between number of followers and whether most popular album is present in that playlist | 3.35 s                        | 18min 39s                    |
| Correlation between number of tracks and number of followers                                       | 1.48 s                        | 9min 20s                     |
| **Search - build index**                                                                           |                               |                              |
| Build reverse lookup from track to list of playlists                                               | 3.25 s                        | 9min                         |
| Find “SongRank”                                                                                    | 28.4 s                        | 11min 27s                    |
| Find keywords from track names and build an inverted index from keyword to list of tracks          | 29 s                          | 1min 25s                     |
| **Search - perform the search**                                                                    |                               |                              |
| Search a song                                                                                      | 4.06 s                        | 4.67 s                       |
| Search and show top 5 playlists                                                                    | 5.12 s                        | 5.46 s                       |
