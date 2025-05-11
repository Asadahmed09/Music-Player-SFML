# OOP Project Report

## Project Title: Smart Music Player using C++ and SFML

## Group Members

- **Asad Ahmed (24k-1013)** — Group Leader
- **Shahnawaz Khuwaja (24k-0791)**
- **Lucky (24k-0865)**
- **Yashraj (24K-0737)**

**Submission Date: May 11, 2025**

## 1\. Executive Summary

Overview:  
Our project is a feature-rich music player built using **C++** and **SFML** (Simple and Fast Multimedia Library). It includes essential audio playback functionality and user-friendly playlist management. To improve the user experience, a graphical interface was designed using SFML’s graphics module. The application supports both a **command-line interface** and a **graphical user interface**, giving flexibility to users. A "MyFavourite" playlist is stored persistently using file handling techniques, allowing the user to retrieve saved playlists upon relaunch.

### Key Achievements

- Implemented core playback functions: **play, pause, resume, stop, next, previous**
- Designed and managed **favorite playlists** using file I/O
- Integrated **SFML** for GUI elements and audio playback (sf::Music)

## 2\. Introduction

Background:  
Music software helps in understanding the integration of multiple OOP principles with multimedia development. This project encapsulates real-world use of C++ classes, file streams, GUI libraries, and sound APIs through SFML.

### Project Objectives

- Develop a music player in C++ using **OOP principles**
- Provide **persistent playlist storage** using file handling
- Design a **graphical interface using SFML**

## 3\. Project Description

Scope:  
Supported Features:

- Play, pause, resume, stop songs
- Add/remove songs from a dynamic “MyFavourite” playlist
- Save/load playlists using file I/O
- Navigate with next/previous options
- GUI controls using **SFML graphics and events**
- Volume control

#### Excluded Features

- Streaming or online support
- Progress bar display
- Dynamic song loading

#### Technical Overview

- **Language:** C++
- **IDE:** Visual Studio Code
- **Sound Engine:** sf::Music from **SFML Audio Module**
- **Graphics/UI:** **SFML Graphics Module** (sf::RenderWindow, sf::Text, sf::RectangleShape)
- **Data Management:** Vectors and file streams (&lt;vector&gt;, &lt;fstream&gt;)
- **File Types Supported:** .wav (compatible with sf::Music::openFromFile)

## 4\. Methodology

### Approach

- Weekly planning with team task lists
- Frequent team meetings for testing and debugging
- Internal discussions for architecture and GUI decisions

### Team Roles

- **Asad Ahmed:** Backend logic, playback integration using SFML, file handling
- **Lucky:** Playlist logic, navigation functions, file persistence
- **Yashraj:** logical functions with SFML
- **Shahnawaz Khuwaja:** Backend logic,GUI implementation and event testing using SFML

## 5\. Project Implementation

### Design and Structure

- OOP-based Action class handles music control
- Songs stored as strings (paths), managed via vectors
- Playlist saved/loaded from MUSICFILE.txt using fstream
- GUI developed using **SFML’s** event loop and render system

### Core Functionalities Developed

- Music playback with sf::Music 
- Add/remove songs to “MyFavourite” playlist
- Save/load playlists using file handling
- Navigation through playlist with next/previous
- GUI buttons for **Play, Pause, Resume, Stop** using mouse events

### Libraries and Headers Used

- &lt;SFML/Audio.hpp&gt;
- &lt;SFML/Graphics.hpp&gt;
- &lt;fstream&gt;, &lt;iostream&gt;, &lt;vector&gt; , &lt;memory&gt; , &lt;functional&gt; , &lt;sstream&gt;

**Challenges Faced:**

- Correct use of sf::Music for real-time audio control
- GUI layout design and button hitbox detection
- Converting audio to .wav and .ogg format for SFML compatibility
- Syncing user actions (mouse clicks) with music states
- Preventing file duplication and managing large playlists

## 6\. Results

### Project Outcomes

- Fully working command-line and SFML-based GUI music player
- Graphical buttons with playback control
- Persistent playlist feature that loads/saves accurately
- Extendable design with modular structure

### Testing and Validation

- Manually tested all playback features
- GUI buttons tested for hover/click state response
- Verified .wav file compatibility and playlist integrity
- File read/write operations tested with valid and invalid inputs

## 7\. Conclusion

Summary of Findings:  
The project successfully achieved the core objectives. It showcases effective use of **Object-Oriented Programming** in C++ alongside real-time **audio playback** and **interactive GUI design** using **SFML**. Core functionalities like play, pause, stop, resume, and playlist persistence were implemented cleanly.

We also planned and partially implemented advanced features like **skip control** and **pitch/speed manipulation**, paving the way for future development.

Final Remarks:  
This music player project was a hands-on journey through multimedia development, OOP concepts, and collaborative teamwork. Each member contributed in distinct ways—from backend audio control to GUI development using SFML.

Challenges like audio format compatibility, UI layout logic, and file management were tackled with consistent teamwork. The SFML framework offered robust tools for audio and graphics, allowing us to move away from Raylib and build a more scalable application.

### Future Enhancements Planned

- Add 10-second skip forward/backward (sf::Time manipulation)
- Implement pitch/speed adjustments with setPitch()
- Improve GUI layout and add animations
