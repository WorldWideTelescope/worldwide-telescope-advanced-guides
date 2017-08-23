#### [Advanced Audio Playback](#AdvancedAudioPlayback)

WorldWide Telescope (WWT) can playback an SMPTE timing track to provide timing control of off-board audio or other SMPTE-controller effects. SMPTE provides a flexible, easy-to-implement control solution; this flexibility makes it possible to setup things in various ways. This document will provide a description of two potential scenarios, but more can be created if these don’t map to your facility.

##### Simple Audio Using Embedded Audio File in WWT Tour

The easiest way to setup a system is for the Master Server to output audio, via analog or digital audio output. The mono or stereo audio tracks are created for narration and music on per-slide or Master-slide basis in the tour – see LINK: Authoring/Dealing with Audio and LINK: Authoring/Editing Audio. Then direct connections between the Master Server and hardware sound system (amplifiers and speakers) takes care of the audio. This is a simple case with few pieces, but is limited by the number of audio channels and potentially the quality of the underlying audio files.

**Note**: For all WWT cluster implementations, Tours that are distributed to Projector Servers have the audio stripped out, to reduce file size and speed updating.

##### Multi-Channel Dome with SMPTE-controlled Audio Server

At some planetaria, such as the Grainger Sky Theater at the Adler Planetarium, they have a configuration with three types of servers: Master, Projector and Audio.

The Master Server controls any number or Projection Servers over the network via WWT and WWT Remote. These controls include:

*   Power control of Projection Servers from Master.
*   Updating Tour and Data from Master to Projection Servers.
*   Synchronization of playback on multiple Projection Servers.

For audio, audio tracks (mono, stereo or multi-channel) are loaded onto a dedicated Audio Server. On the WWT Master Server the normal audio track is replaced with a SMPTE timing track. This is usually done with a short-duration slide at the beginning of the tour that is a master and has the SMPTE track as MP3 or WAV format. The analog audio output of the Master Server is connected to an input port on the Audio Server. Once the appropriate audio track(s) are loaded on the Audio Server and the Audio Server is setup to be controlled by input SMPTE timing from Master (via analog audio connections), the audio and video are synchronized via the Master Server.

**Note**: Currently, the timing of WWT cannot be controlled by an external SMPTE source, such as a stand-alone SMPTE generator or Audio Server.
