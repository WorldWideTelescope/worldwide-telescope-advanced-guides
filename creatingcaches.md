#### [Creating WorldWide Telescope Caches](#creatingcaches)

#### Overview

WorldWide Telescope (WWT) is a great tool with access to Petabytes of image data from the cloud, but in some educational contexts the internet may not be available but it is desirable to use WWT as a tool on a stand-alone basis. WorldWide Telescope already can operate off-line when the internet is available, and browse any data previously viewed by that user on that machine. In a new installation, there is no cache history for a user to rely on and the experience is not acceptable.

To solve this issue we have created a tool that will allow for the creation of curated cache content that would be installed from a DVD or thumb drive along with the WWT client to allow a disconnected or poorly connected machine to run most of WWT features without ever having to connect to the internet.

#### Tools

WWT already has existing tools for basic cache management. With the Eclipse release WWT adds several new tools to help curate the cache contents. This is a combined list of both the new and old tools.

*   Cache measurement/purge utility in the Settings tab
*   Cache Management Menu from Right click menu item in explore/context tabs.
    *   Cache Image Tile Pyramid
    *   Show Cache Space Used
    *   Remove from Image Cache
*   Playing a tour caches all data it views.
*   Playing tours with “Play all” option will play and repeat tours in a collection
*   Browsing collections will add images you view to the cache.
*   Play collection as slideshow will go from image to image and cache data as it goes.
*   Editing the cache directory manually thru Windows explorer.
    *   C:\Users\{user name here}\AppData\Local\Microsoft\WorldWideTelescope
*   Setting up WMS servers, and caching data they use.
*   Running WWT in Solar System mode with Multi-Resolution planets will load in base maps need for that mode.
*   Save the Cache in Settings…Advanced..Save Cache as Cabinet File…
*   Load the Cache in Settings…Advances…Restore Cache from Cabinet File…

#### Process

1.  Ensure your WWT instance has a fresh, clean cache.
2.  Use the cache tools to load data you thing is important .
3.  Measure the cache size as you go budgeting for the data sets you need.
4.  Use the UI or manual cache management in Explorer to trim excess if needed.
5.  Save The Cache file to a cabinet file.
6.  Move the cabinet file to a fresh non-internet connected machine.
7.  Install a fresh WWT install.
8.  Restore the Cabinet file.
9.  Verity operation and note any missing data.
10.  Repeat the above steps as necessary until the cache meets the educational requirements.

#### Deployment

In the final Eclipse release the setup will detect the presence of a cache cabinet file and offer to install it automatically. This file should be named “WwtFileCache.cabinet” and be placed next to the WWTSetup.5.x.x.msi file. After installation WWT will use this cache transparently as if it actually visited all the data already.

<video id="cachemgt" controls="" width="100%" class="img-responsive"><source src="@Model.ContentDir/videos/cachemanagement.ogv" type="video/ogg; codecs=&quot;theora, vorbis&quot;"> <source src="@Model.ContentDir/videos/cachemanagement.webm" type="video/webm"> <source src="@Model.ContentDir/videos/cachemanagement.mp4" type="video/mp4">

Video is not visible, most likely your browser does not support HTML5 video

</video>
