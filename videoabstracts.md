#### [Making Video Abstracts with WWT](#videoabstracts)

### Pre-flight Question:

Can one or more images be used as a primary way to communicate the main science result?

If the answer is no, it will be difficult to make a video abstract completely with WWT.  It will take more time and WWT could be used for parts, but final abstract would have most of the visuals created outside of WWT and edited together.

If yes, keep reading.

### Overview

Total Time about 6 - 14 hr

1.  Prepare data: 0 - 4 hr
2.  Make story board: 0.5 hr
3.  Write draft script: 1 hr
4.  Record draft narration: 0.5 hr
5.  Create draft tour: 1 - 3 hr
6.  Create draft video [OPTIONAL]: 0.5 hr
7.  Sharing and feedback: 1.0 hr
8.  Record final narration: 0.5 -1.5 hr
9.  Refine tour: 1 - 2 hr
10.  Create final video [OPTIONAL]: 0.5 hr

Appendix A: Limitation of the web-based tour player

Appendix B: Using Communities

### 1 Prepare data

#### Estimated Time: 0-4 hr

#### Tools: FITS Liberator ([http://www.spacetelescope.org/projects/fits_liberator/](http://www.spacetelescope.org/projects/fits_liberator/)), Adobe Photoshop, Adobe Illustrator

Some abstracts can be presented with the data in WWT, adding only text and image overlays.  Other, more complex tours will want to represent the original new data presented in the paper.  In these cases, significant time might have to be taken to import FITS or other data formats into WWT.

Below is one representative workflow used to get the data into WWT necessary for a video abstract.  This workflow assumes that the data that will be added to WWT in order to present the abstract are in the form of FITS files.  More detailed instructions on loading images are available here: [http://www.worldwidetelescope.org/Learn/Exploring#AstroImageData](http://www.worldwidetelescope.org/Learn/Exploring#AstroImageData). 

1.  Use FITS Liberator ([http://www.spacetelescope.org/projects/fits_liberator/](http://www.spacetelescope.org/projects/fits_liberator/)) to make TIFF from original FITS file.
    1.  Had to select "No Flip" (which controls vertical flips)
    2.  The image was still flipped horizontally, so…
    3.  Loaded output TIFF into Photoshop and did a horizontal flip and resaved
2.  Test by loading large TIFF into WWT
3.  When final TIFFs are made, post TIF on website e.g., [http://jansky.phys.northwestern.edu/wwt/Sgr_A_West-Ka.tif](http://jansky.phys.northwestern.edu/wwt/Sgr_A_West-Ka.tif). Note that since the TIF file was derived from a very large image, the output TIF file is also large – 450 MB.
4.  Import the image into WWT (i.e., process TIFF to create a multiresolution version of the data in TOAST format), [http://worldwidetelescope.org/interact/embed](http://worldwidetelescope.org/interact/embed)
5.  Return collection (WTML file) which has reference to new tiled images that can now be used in a tour.

In the example, this was done for two images.  One was the astronomical VLA image “Sgr_A_West-Ka” and the second was a line plot.  For the plot, the coordinates were copied from an image at the same scale. The plot was exported from Illustrator as a PNG with transparency everywhere except where the lines of the plot were to be drawn.

You can also add other types of data:

*   Pointed images (i.e., FITS, see above): [http://www.worldwidetelescope.org/Learn/Exploring#AstroImageData](http://www.worldwidetelescope.org/Learn/Exploring#AstroImageData)
*   Web Map Service (mostly for layer data on the surface of the Earth) [http://www.worldwidetelescope.org/Learn/Exploring#AddingWMSData](http://www.worldwidetelescope.org/Learn/Exploring#AddingWMSData)
*   Catalogs and tabular information: [http://www.worldwidetelescope.org/Learn/Exploring#UsingVOTables](http://www.worldwidetelescope.org/Learn/Exploring#UsingVOTables)
*   Panoramic images (e.g., panorama of observatory): [http://www.worldwidetelescope.org/Learn/Exploring#processingpanoramas](http://www.worldwidetelescope.org/Learn/Exploring#processingpanoramas)
*   All-sky images (e.g., any all-sky map not already in WWT): [http://www.worldwidetelescope.org/Learn/Exploring#processingallskyimages](http://www.worldwidetelescope.org/Learn/Exploring#processingallskyimages)

### 2 Make story board

#### Estimated Time: 0.5 hr

The story board is a sequence of draft visuals representing what will be on screen.  It can be in the form of descriptions of what is to be shown or a list of figures (from WWT as well as those in the paper).  In the case of the example Proplyd paper, it was a list of figures, selecting those from the paper that directly supporting the words of the written abstract (script of the tour).

### 3 Write draft script

### Estimated Time: 1 hr

Drafting a script in either bullet or written form is the first step in the process.  The simplest way to do this is to read the written abstract with modest revisions for acronyms, jargon and detailed numerical data.  In an example, reading the text of the abstract verbatim took about 2:15.  It is probably easier to start by using a template for script and story board.  A template is available here: **Tour Template.docx** and an example script is available here: **Video Abstract - Proplyd - v1.1.docx.**

### 4 Record draft narration

#### Estimated Time: 0.5 hr

#### Tools: Audacity ([http://audacity.sourceforge.net](http://audacity.sourceforge.net))

Record draft narration for timing.  Don’t worry about flubs or mistakes as long as they don’t change the time appreciably.  It is suggested to use Audacity ([http://audacity.sourceforge.net](http://audacity.sourceforge.net)), which is a free tool available on Mac OS, Linux or Windows to record and edit audio.  However, feel free to use any program that can create a high-quality MP3 file.  There are on-line tutorials on how to create audio:

*   [http://www.worldwidetelescope.org/Learn/Authoring#dealingwithaudio](http://www.worldwidetelescope.org/Learn/Authoring#dealingwithaudio)
*   [http://www.worldwidetelescope.org/Learn/Authoring#editingaudio](http://www.worldwidetelescope.org/Learn/Authoring#editingaudio)

### 5 Create draft tour

#### Estimated Time: 1-3 hr

#### Tools: WorldWide Telescope ([http://www.worldwidetelescope.org](http://www.worldwidetelescope.org))

Create a draft tour showing visuals timed to draft narration.  Work is on-going to enable creation of tours in the web client, but for now, you must use the Microsoft Windows Desktop client ([http://www.worldwidetelescope.org](http://www.worldwidetelescope.org)) to author your tour.  Note that there are two type of tours. The simplest is a “slide-based tour” which is composed of a sequence of slides, each with a begin and end position.  The visualizations are interpolated between the beginning and end of each slide.  Slide-based tours can be played back in the web tour player or the Windows Desktop client. 

There is a more advanced type of tour called a keyframe-based (or timeline).  Keyframe-based tours provide fine-grained control over the tour with the ability to specify any parameter at any time (down to 1/30 of a second).  Timeline based tours can provide more cinematic tours but cannot be played back in the web tour player and can only be shared on-line in the form of videos.  Since much of the power of WWT-based video abstracts comes from comparing data supporting the journal article with other data, you should create your tour as a slide-based tour.  After this is created for your paper, you can convert a slide-based tour into a timeline one in order to make a more polished video but the tour directly related to your paper would be the slide-based, web-playable version.

There is more information on creating slide-based tours here: [http://www.worldwidetelescope.org/Learn/Authoring#slidebasedtours](http://www.worldwidetelescope.org/Learn/Authoring#slidebasedtours)

When you are finished with the tour, make sure to save your tours with good naming and versioning information to help organize your files as you refine in the later steps.

### 6 Create draft video (optional)

#### Estimated Time: 0.5 hr

#### Tools: Adobe Premiere, Apple QuickTime or FFmpeg (http://ffmpeg.org/)

You have to use the Windows Desktop client to render the tour to a sequence of image frames (PNG).  Instructions on that are available here:

*   [http://www.worldwidetelescope.org/Learn/Authoring#rendertovideo](http://www.worldwidetelescope.org/Learn/Authoring#rendertovideo)

Once you have the frames, you need to use a program to take that and the audio narration and encode them as a video.  This is straightforward to do with a modern video encoder, such as Adobe Premiere.  It is also possible to use the cheap Apple QuickTime program to do this.  This process may take a while to complete, but user interaction time is modest.  When complete, you will likely want to post your video YouTube or similar video sharing service to share with your colleagues for feedback. 

### 7 Sharing & Feedback

#### Estimated Time: 1.0 hr

Share your tour with colleagues (e.g., co-authors on paper) to get feedback.  Sharing the tour can be done in one of a few ways:

1.  If they have a Windows PC with WWT installed, you can share the tour file itself, which should be small unless you have many high-resolution images included.
2.  You can also share the YouTube video link if you did the optional step of making a video from the tour (see Section 6 above). This of course can be viewed on most desktop and mobile devices.
3.  You can also create a community ([http://worldwidetelescope.org/Learn/Authoring#usingcommunities](http://worldwidetelescope.org/Learn/Authoring#usingcommunities) – also included as Appendix B below).  From here you can share a link directly or you can have your colleagues join the community.

Organize the responses and make clear choices about what you will change to address them.  This is likely to be in form that you assumed the viewer would know something and need to add descriptive text on screen or in narration for those that don’t.  This will likely require changes to the script as well as tour (timing and adding text labels, data etc.).

### 8 Record final narration

#### Estimated Time: 0.5 – 1.5 hr

Refine script and record new audio based on feedback.  You will use the same tools as you did to record the draft narration.  However, you will want to get a high a quality recording as possible (good microphone, quiet room, a fresh voice).  You may want to embellish the narration with a music or ambient sound bed.  If you do add music, make sure that is low in volume, compared to the narration.

### 9 Refine tour

#### Tools: WorldWide Telescope ([http://www.worldwidetelescope.org](http://www.worldwidetelescope.org))

#### Estimated Time: 1 - 2 hr

Refine tour base on feedback.  Use the final audio for final timings.  Slide lengths may need be changed to accommodate changes in narration timing.  Also

### 10 Create final video (optional)

#### Tools: Audacity ([http://audacity.sourceforge.net](http://audacity.sourceforge.net))

#### Estimated Time: 0.5 hr

Using the same work flow as you did to create the draft video, create the final one.   The steps are essentially the same.

* * *

### Appendix A: Limitation of the web-based tour player

Some tours can be played back in a web-based Tour player.  You can put your tour on some website (e.g., [http://jansky.phys.northwestern.edu/Video_Abtract-Proplyd.wtt](http://jansky.phys.northwestern.edu/Video_Abtract-Proplyd.wtt)) and then point embed the code to play the tour in the web-based Tour player here:

*   [http://worldwidetelescope.org/interact/embed](http://worldwidetelescope.org/interact/embed)

You can try to play the tour by embedding this code into a web-site and viewing the page.

Below is a non-exhaustive list of issues about Tours in the web player:

*   Audio must be one audio file for complete tour (can’t be separate ones per slide and can’t be separate music and narration)
*   Audio must be in MP3 format.
*   Only sky mode is allowed.
*   Can’t use layered data.
*   Can’t use timeline.
