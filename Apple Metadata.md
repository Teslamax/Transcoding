# Quick Reference Sheet for Media Metadata and Device Compatibility

## Video and Audio Metadata for *Apple TV* and *Music App*

### Apple TV Metadata Table (Video)

| **Field**              | **Description**                                                                 | **Technical Name**         | **Example Data**          | **Required** |
|------------------------|---------------------------------------------------------------------------------|----------------------------|---------------------------|--------------|
| **Title**              | The name of the video.                                                           | `title`                    | `The Great Adventure`     | ✔            |
| **Genre**              | The genre of the video content.                                                   | `genre`                    | `Comedy`                  |             |
| **Artwork/Poster**     | The image representing the video (e.g., video thumbnail).                        | `artwork`                  | `cover.jpg`               |              |
| **Subtitle/Caption Tracks** | Text tracks for subtitles or closed captions.                                   | `subtitle`                 | `english.srt`             |              |
| **Release Date**       | The date the video was released.                                                | `release_date`             | `2023-05-15`              |              |
| **Season and Episode Numbers** | Used for TV shows to categorize by season and episode.                       | `season_number`, `episode_number` | `Season 1`, `Episode 5` |              |
| **Resolution**         | The resolution of the video (e.g., 1080p, 4K).                                   | `resolution`               | `1080p`                   |              |
| **Aspect Ratio**       | The aspect ratio of the video (e.g., 16:9, 4:3).                                 | `aspect_ratio`             | `16:9`                    |              |
| **Bitrate**            | The video bitrate used for encoding.                                            | `bitrate`                  | `2500k` (video)           |              |
| **Video Mode**         | The mode used for video (e.g., HDR, Standard).                                  | `video_mode`               | `HDR`                     |              |

### Apple Music Metadata Table (Audio)

| **Field**              | **Description**                                                                 | **Technical Name**         | **Example Data**          | **Required** |
|------------------------|---------------------------------------------------------------------------------|----------------------------|---------------------------|--------------|
| **Title**              | The name of the audio track.                                                     | `title`                    | `The Great Adventure`     | ✔            |
| **Artist**             | The performer or band for audio.                                                 | `artist`                   | `John Doe`                | ✔            |
| **Album**              | The album name for audio.                                                        | `album`                    | `Summer Hits`             | ✔            |
| **Genre**              | The genre of the audio content.                                                   | `genre`                    | `Comedy`                  | ✔            |
| **Artwork/Poster**     | The image representing the audio (e.g., album art).                             | `artwork`                  | `cover.jpg`               |   ✔          |
| **Track Number**       | The track number in an album (for audio).                                        | `track_number`             | `5`                       |              |
| **Album Artist**       | The artist or group for an album (for compilations).                             | `album_artist`             | `Various Artists`         |              |
| **Composer**           | The composer of the music (for classical works).                                 | `composer`                 | `Beethoven`               |              |
| **Year**               | The year the album or track was released.                                        | `year`                     | `2023`                    |              |
| **Language**           | The language the audio content is in.                                            | `language`                 | `English`                 |              |
| **Rating**             | User-assigned rating for the media (1–5 stars).                                  | `rating`                   | `5`                       |              |
| **Copyright**          | Copyright information for the content.                                           | `copyright`                | `© 2023 John Doe Music`   |              |
| **Grouping**           | Used to group tracks (e.g., remixes, collections).                              | `grouping`                 | `Remixes`                 |              |
| **Sampling Rate**      | The audio sampling rate (e.g., 44.1 kHz, 48 kHz).                               | `sampling_rate`            | `44.1kHz`                 |              |
| **Bit Depth**          | The bit depth for audio (e.g., 16-bit, 24-bit).                                  | `bit_depth`                | `16-bit`                  |              |

### Automatically Determined Metadata (Read-Only)

| **Field**              | **Description**                                                                 | **Technical Name**         | **Example Data**          |
|------------------------|---------------------------------------------------------------------------------|----------------------------|---------------------------|
| **Video Codec**        | The codec used for encoding the video (e.g., H.264, HEVC).                       | `video_codec`              | `H.264`                   |
| **Audio Codec**        | The codec used for encoding the audio (e.g., AAC, MP3, ALAC).                    | `audio_codec`              | `AAC`                     |
| **File Format**        | The container type of the media file (e.g., MP4, MP3, AAC).                     | `format`                   | `MP4`                     |
| **Duration**           | The total length of the video/audio in seconds.                                   | `duration`                 | `3600` (1 hour)           |

---

### Common Encoders and Profiles Supported by Your Devices

| **Device**               | **Video Encoders**         | **Supported Profiles**                           | **Audio Encoders** | **Supported Audio Profiles** |
|--------------------------|----------------------------|--------------------------------------------------|--------------------|------------------------------|
| **MacBook Pro 2018 (13")** | H.264, HEVC (H.265), VP9    | H.264 High, HEVC Main, HEVC Main 10             | AAC, MP3, ALAC     | AAC Low Complexity (LC), MP3 |
| **iPhone 15 Pro Max**     | H.264, HEVC (H.265), VP9    | H.264 High, HEVC Main, HEVC Main 10             | AAC, MP3, ALAC     | AAC Low Complexity (LC), MP3 |
| **iPad Air 5th Gen (M1)** | H.264, HEVC (H.265), VP9    | H.264 High, HEVC Main, HEVC Main 10             | AAC, MP3, ALAC     | AAC Low Complexity (LC), MP3 |
| **Amazon Fire Cube (2nd Gen)** | H.264, HEVC (H.265), VP9    | H.264 Main, HEVC Main                          | AAC, MP3, Dolby Digital (AC-3) | AAC, MP3, Dolby Digital (AC-3) |

### Common Containers and Codec Formats

| **Container**  | **Commonly Used Codecs**                             | **Device Compatibility**    |
|----------------|------------------------------------------------------|-----------------------------|
| **MP4**        | H.264, HEVC (H.265), AAC, MP3, ALAC                  | Apple TV, iPhone, iPad, Fire Cube |
| **MOV**        | H.264, HEVC (H.265), AAC, MP3, ALAC                  | Apple TV, iPhone, iPad      |
| **MKV**        | VP9, H.264, HEVC, AAC, MP3                           | Apple TV (via third-party apps), Fire Cube (via third-party apps) |
| **AVI**        | H.264, MP3                                           | Limited to third-party apps on all devices |
| **WebM**       | VP9, Opus                                            | Fire Cube (via third-party apps) |

---

# Predefined Metadata Tags for Apple TV and Apple Music

## Apple TV and Apple Music Metadata Tags

### **Genre (Audio - Apple Music)**

| **Accepted Values**                     |
|-----------------------------------------|
| Pop, Rock, Hip-Hop/Rap, Classical, Jazz, Electronic, Alternative, Country, Blues, R&B, Reggae, Folk, Indie, Soundtrack, Comedy, Children’s Music, Holiday, Latin, Christian & Gospel, New Age |

### **Content Rating (Video - Apple TV)**

| **Accepted Values**                      |
|------------------------------------------|
| G, PG, PG-13, R, NC-17, TV-Y, TV-G, TV-PG, TV-14, TV-MA |

### **Media Kind (Audio - Apple Music)**

| **Accepted Values**                  |
|--------------------------------------|
| Music, Audiobook, Podcast, Movie, TV Show, Home Video |

### **TV Show Episode (Video - Apple TV)**

| **Description**             |
|-----------------------------|
| **Season Number**: e.g., 1, 2, 3  |
| **Episode Number**: e.g., 1, 2, 3  |

### **Language (Video and Audio - Apple TV & Apple Music)**

| **Accepted Values**           |
|-------------------------------|
| en (English), es (Spanish), fr (French), de (German), it (Italian), ja (Japanese), pt (Portuguese), zh (Chinese), ru (Russian), ko (Korean), ar (Arabic), hi (Hindi) |

### **Movie Type (Video - Apple TV)**

| **Accepted Values**        |
|----------------------------|
| Feature Film, Short Film, Documentary, Animated |


### Conclusion

This quick-reference sheet provides an overview of the **metadata** fields required for **Apple TV** and **Apple Music** (formerly iTunes) app compatibility, along with the **supported encoders** and **profiles** for each of your devices. You can refer to this sheet for easy encoding and transcoding decisions, ensuring the best compatibility and performance for your videos and audio content.
