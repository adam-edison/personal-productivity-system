# Personal Productivity System

A full-blown productivity system using:

* Tasks
* Subtasks
* Habits
* Procedures
* Goals
* Achievements

All managed by voice. Designed to reduce screen time and save you time overall!

This system is reliant upon quite a few locally-running services on Mac OS.

* [Talkback Node Server](https://github.com/adam-edison/talkback-node-server)
  * for Text to Speech (TTS), 100% free
  * Runs locally on Mac OS
* [AudioRelay](https://audiorelay.net/)
  * for using phone (with or without bluetooth headphones) as a microphone
  * for using phone (with or without bluetooth headphones) as an audio output device
  * Runs locally on Mac OS
* [Blackhole Audio](https://existential.audio/blackhole/)
  * for creating 0-latency audio devices on Mac (using both 2 and 16 channel devices)
  * 2 channel is for mic (phone to Mac)
  * 16 channel is for audio output (Mac to phone)
  * Both run as virtual audio devices on Mac OS
* [Personal Productivity System](https://github.com/adam-edison/personal-productivity-system)
  * uses [Docker Desktop](https://www.docker.com/products/docker-desktop/) for local Postgres database
  * Runs locally on Mac OS
  * stores data and provides API (and features) for advanced tasks, habits, procedures, goals and achievements
* [Talon Voice](https://talonvoice.com/)
  * voice commands contained here
  * source of REST API requests to Talkback Node Server
  * source of REST API requests to Personal Productivity System
