# Quick Reference Sheet for Video and Audio Metadata and Device Compatibility

## Video and Audio Metadata for Apple TV and Music App

### Video Metadata Table (Apple TV App)

| **Field**              | **Description**                                                                 | **Technical Name**         | **Example Data**          | **Mandatory/Optional** | **Automatically Determined**        |
|------------------------|---------------------------------------------------------------------------------|----------------------------|---------------------------|------------------------|--------------------------------------|
| **Title**              | The name of the video or audio track.                                             | `title`                    | `The Great Adventure`     | **Mandatory**           | No                                   |
| **Artist**             | The performer or band for audio.                                                 | `artist`                   | `John Doe`                | **Mandatory** (Audio)   | No                                   |
| **Album**              | The album name for audio.                                                        | `album`                    | `Summer Hits`             | **Mandatory** (Audio)   | No                                   |
| **Genre**              | The genre of the content.                                                         | `genre`                    | `Comedy`                  | **Mandatory** (Audio/Video) | No                                   |
| **Duration**           | The total length of the video/audio in seconds.                                    | `duration`                 | `3600` (1 hour)           | **Mandatory**           | Yes                                  |
| **File Format**        | The container type of the media file (e.g., MP4).                                | `format`                   | `MP4`                     | **Mandatory**           | Yes                                  |
| **Video Codec**        | The codec used for encoding video (e.g., H.264 or HEVC).                         | `video_codec`              | `H.264`                   | **Mandatory** (Video)   | Yes                                  |
| **Audio Codec**        | The codec used for encoding audio (e.g., AAC, MP3, ALAC).                        | `audio_codec`              | `AAC`                     | **Mandatory** (Audio/Video) | Yes                                  |
| **Artwork/Poster**     | The image representing the content (e.g., album art or video thumbnail).         | `artwork`                  | `cover.jpg`               | **Optional**            | No                                   |
| **Subtitle/Caption Tracks** | Text tracks for subtitles or closed captions.                                   | `subtitle`                 | `english.srt`             | **Optional**            | No                                   |
| **Release Date**       | The date the video or music was released.                                        | `release_date`             | `2023-05-15`              | **Optional**            | No                                   |
| **Season and Episode Numbers** | Used for TV shows to categorize by season and episode.                       | `season_number`, `episode_number` | `Season 1`, `Episode 5` | **Optional**            | No                                   |
| **Resolution**         | The resolution of the video (e.g., 1080p, 4K).                                   | `resolution`               | `1080p`                   | **Optional**            | No                                   |
| **Aspect Ratio**       | The aspect ratio of the video (e.g., 16:9, 4:3).                                 | `aspect_ratio`             | `16:9`                    | **Optional**            | No                                   |
| **Bitrate**            | The video or audio bitrate used for encoding.                                    | `bitrate`                  | `2500k` (video), `256k` (audio) | **Optional**            | No                                   |
| **Video Mode**         | The mode used for video (e.g., HDR, Standard).                                  | `video_mode`               | `HDR`                     | **Optional**            | No                                   |
| **Track Number**       | The track number in an album (for audio).                                        | `track_number`             | `5`                       | **Optional** (Audio)    | No                                   |
| **Album Artist**       | The artist or group for an album (for compilations).                             | `album_artist`             | `Various Artists`         | **Optional** (Audio)    | No                                   |
| **Composer**           | The composer of the music (for classical works).                                 | `composer`                 | `Beethoven`               | **Optional** (Audio)    | No                                   |
| **Year**               | The year the album or movie was released.                                        | `year`                     | `2023`                    | **Optional** (Audio/Video) | No                                   |
| **Language**           | The language the content is in.                                                  | `language`                 | `English`                 | **Optional**            | No                                   |
| **Rating**             | User-assigned rating for the media (1–5 stars).                                  | `rating`                   | `5`                       | **Optional**            | No                                   |
| **Copyright**          | Copyright information for the content.                                           | `copyright`                | `© 2023 John Doe Music`   | **Optional**            | No                                   |
| **Grouping**           | Used to group tracks (e.g., remixes, collections).                              | `grouping`                 | `Remixes`                 | **Optional** (Audio)    | No                                   |
| **Sampling Rate**      | The audio sampling rate (e.g., 44.1 kHz, 48 kHz).                               | `sampling_rate`            | `44.1kHz`                 | **Optional** (Audio)    | No                                   |
| **Bit Depth**          | The bit depth for audio (e.g., 16-bit, 24-bit).                                  | `bit_depth`                | `16-bit`                  | **Optional** (Audio)    | No                                   |
| **Video Codec**        | The codec used for encoding the video (e.g., H.264, HEVC).                       | `video_codec`              | `H.264`                   | **Automatically Determined** | Yes                                  |
| **Audio Codec**        | The codec used for encoding the audio (e.g., AAC, MP3, ALAC).                    | `audio_codec`              | `AAC`                     | **Automatically Determined** | Yes                                  |
| **File Format**        | The container type of the media file (e.g., MP4).                                | `format`                   | `MP4`                     | **Automatically Determined** | Yes                                  |
| **Duration**           | The total length of the video/audio in seconds.                                   | `duration`                 | `3600` (1 hour)           | **Automatically Determined** | Yes                                  |

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

### Conclusion

This quick-reference sheet provides an overview of the **metadata** fields required for Apple TV and Music app compatibility, along with the **supported encoders** and **profiles** for each of your devices. You can refer to this sheet for easy encoding and transcoding decisions, ensuring the best compatibility and performance for your videos and audio content.

---

Once you're satisfied with the **Markdown version**, let me know, and I'll generate the **PDF version** for you!
