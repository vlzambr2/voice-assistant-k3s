# Voice Assistant K3s

Kubernetes object definitions for a local Voice Assistant pipeline integrated with Home Assistant and Music Assistant. This setup enables locally hosted music playback by voice, leveraging components such as Faster Whisper, Open Wake Word, and YouTube Music.

This project demonstrates a **microservices architecture** using Kubernetes.

> This repository is designed specifically for a Kubernetes cluster running entirely on the **Bunny Computer**, and as such, contains configuration-specific details such as node names and host paths. For more information, see [Bunny Computer-Specific Configuration](#bunny-computer-specific-configuration).

## Integrations

- **Music Assistant**: Local music playback with YouTube Music support.
- **Voice Assistant Pipeline**: Faster Whisper and Open Wake Word for wake word detection and speech transcription.
- **VLC Telnet**: Service providing access to speakers connected to Pi 3mm jack. 
- **Home Assistant**: Voice assistant conversation agent and connective tissue between all services.

## Notes
* [Music Playback Voice Control](https://github.com/music-assistant/voice-support) Home Assistant blueprint applied to enable voice control of Music Assistant.
* Google TTS used for text-to-speech.

## Acknowledgments

- [Home Assistant](https://www.home-assistant.io/)
- [Music Assistant](https://github.com/music-assistant)
- [Faster Whisper](https://github.com/guillaumekln/faster-whisper)
- [Open Wake Word](https://github.com/rhasspy/openwakeword)

## Bunny Computer-Specific Configuration

This Kubernetes cluster is configured to run entirely on the **Bunny Computer**. 

The Bunny Computer is a Pi cluster originally created in 2022 to use [Chapel](https://chapel-lang.org/) (open-source-parallel-programming language) to ["rip" CD .flac files in parallel](https://github.com/vlzambr2/process_album)-- now promoted to the role of home server!  **₍ᐢ. .ᐢ₎.** 

For more info about the Bunny Computer, visit [my personal website](https://www.vanessaz.info/pages/bunnycomputer).