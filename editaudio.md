#### [Editing Audio](#editingaudio)

In the Dealing with Audio how-to, we show how to get audio tracks into WWT. This guide will give some tips on how to create and edit the audio that you want to include in your tour. WWT can play a variety of audio files. Playback quality it limited to the quality of the input audio file so start with the highest quality. If you are getting an existing file or if you are creating your own try to get a lossless format, like WAV, or a high-bitrate one, like 320 kbps MP3\.

I will illustrate how to edit audio using an open source windows program called Audacity (http://audacity.sourceforge.net/), however most audio editing software can probably do the same things.

I edit software for the following purposes: trimming, normalization, background noise removal and format conversion. I would do all editing in WAV and then convert to MP3 at the last step. Also, I would use draft audio until you have finalized the visual timing and then do audio editing and conversion.

#### Trimming

When you get music of narration files often the timing of the files needs to be adjusted. When you know the timing of the tour you are trying to match and the audio file you may need to cut some off of the audio file. Cutting the length for the file can make is smaller and you can also add custom fades (in and out) at this point.

Figure out the time you want to trim to and if you want to add a fade in or fade out. For this example I will put a 2 second fade out at the end of a musical audio file. Since the music builds gradually, I will not change the beginning of that with a fade-in.

1.  Open Audacity and load input audio file. Identify the length you want the audio piece to be.
2.  Use mouse to select 2 seconds from the end.
3.  Click “Effect” in the top menu and select “Fade Out.” This will create a linear fade out that you can see graph in Audacity.
4.  Select from the beginning to the end of the ending fade.
5.  Click “File” in menu and “Export Selection.”
6.  Choose WAV -- assuming you will save this uncompressed WAV file as an archive and convert to MP3 in another step (see below).

#### Normalization

Audio is inherently analog and capturing a digital copy requires you to sample it into a range of digital values. Digitized signals have specific steps between each level. In order to have the best sounding signal it should be normalized such that the maximum signal is at the highest value of the digital signal. This has the effect of making the signal as loud as it can be without clipping. Then you can reduce the volume with the slider in WWT.

1.  Open Audacity and load input audio file. Identify the length you want the audio piece to be.
2.  Use mouse to select the entire file (or the part you want to export and use).
3.  Click “Effect” in the top menu and select “Normalize.” This will bring up a dialog box. I check all boxes and set the maximum amplitude to 0.0 dB. This will scan the file and determine the scaling to amplify the signal to the maximum values.
4.  Select from entire file of a selection.
5.  Click “File” in menu and “Export Selection.”
6.  Choose WAV -- assuming you will save this uncompressed WAV file as an archive and convert to MP3 in another step (see below).

#### Background Noise Removal

1.  Open Audacity and load input audio file.
2.  Put cursor in file window and select a part of the audio file where there is noise. You may want to expand the range to see this clearly.
3.  Click “Effect” in the top menu and select “Noise Removal…” This will bring up a dialog box. Click “Get Profile.”
4.  Then select the entire audio file (or the part you want to save out).
5.  Click “Effect” in the top menu and select “Noise Removal…” This will bring up a dialog box. I leave the default values and then make sure “Remove” is selected and click the “OK” button.
6.  Click “File” in menu and “Export Selection.”
7.  Choose WAV -- assuming you will save this uncompressed WAV file as an archive and convert to MP3 in another step (see below).

#### Format Conversion

If you are getting music files, WAV files are great for quality, but can be large. Note, that tours encapsulate assets like audio and images so be aware that file sizes could be large if you include uncompressed audio like WAV. I suggest working with WAV files and keeping copies of those around for editing, but before putting the files into WWT, converting it to compressed MP3\. Audacity can read in almost any format file and you can select the same file for export to another format.

1.  Open Audacity and load input audio file.
2.  Put cursor in file window and Control-A (select all).
3.  Under “File” click “Export Selection.”
4.  In the dialog box that comes up, select “MP 3 Files” as output format.
5.  Click the “Options” button which opens a box to select MP3 output encoding options. I use Variable Bit Rate, Quality level 5, 110-150 kbps. You can also use Constant Bit Rate with 128 kbps or higher.
6.  Load the file into WWT and play it back to make sure it sounds ok. If you are in a very quiet room with good acoustics and speakers you might hear MP3 compression and want to use a higher bit rate. Note that variable bit rate MP3 use file space a bit more efficiently and plays fine in WWT.
