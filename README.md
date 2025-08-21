# Trailer Audio Editing Project

## 📌 Description
This project demonstrates audio editing using **Audacity** and video processing with **FFmpeg**.  
The main objective is to apply effects to an audio track (trailer soundtrack), export it, and synchronize it with the original video.  

## 🎯 Objectives
- Learn how to edit audio using **Audacity** (apply reverb and other effects).  
- Export the edited track in `.mp3` format.  
- Merge the processed audio with a video trailer using **FFmpeg**.  

## 🛠️ Tools Used
- **Audacity** (for audio editing)  
- **FFmpeg** (for video + audio merging)  

## 📂 Project Files
- `videoplayback.mp4` → Original trailer video.  
- `tron_funny.mp3` → Edited audio file with effects.  
- `final_trailer.mp4` → Final exported trailer with modified soundtrack.  

## 🚀 How to Reproduce
1. Open the trailer audio in **Audacity**.  
2. Apply desired effects (e.g., reverb with 15% room size and 1.2s decay).  
3. Export the audio as `tron_funny.mp3`.  
4. Use **FFmpeg** to merge audio and video:  

   ```bash
   ffmpeg -i videoplayback.mp4 -i tron_funny.mp3 -map 0:v -map 1:a -c:v copy -shortest final_trailer.mp4

👤 Project Member
- Joan Emmanuel Umaña Grajales
