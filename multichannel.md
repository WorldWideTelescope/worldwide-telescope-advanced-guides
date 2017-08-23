#### [Multi-Channel Setup](#multichannel)

This guide is intended to provide a simple path for planetarium setups. It assumes that you aren’t very familiar with WorldWide Telescope (WWT) in domes and steps you through setting it up, loading and playing a tour designed for domes. This guide is meant to be a starting place and is not exhaustive.

Digital planetarium systems are either single computer, which can drive a single projector or cluster of computers which is needed to drive multiple projectors. WWT can be used in both situations. Most steps are common but we describe the two scenarios separately.

**Note:** There is no special dome version of WWT.

### Single Computer Quick Start

This is the simplest setup and has a single computer with two video outputs. One output acts as the console and the other drives the projector that drives the some through a fisheye lens or spherical mirror.

1.  Get the hardware ready.
    1.  Make sure the computer is setup with the primary display connected to a desktop monitor and the secondary display connected to the projector powering the dome.
    2.  Also, make sure the audio output of the computer is connected to a dome audio system.
    3.  Connect the computer to the network.
2.  Install the latest build of WWT - [http://worldwidetelescope.org/Download/](/Download/).
3.  Startup WWT.
4.  Setup Dome. **View/Full Dome/Dome Setup**. Under Dome Type, you can select “FishEye,” “Mirrordome 16:9” or “Mirrordome 4:3.” You can also set the Dome Tilt.
5.  Send dome view to projector by selecting **View/Full Dome/Detatch Main View to Second Monitor**. You should see the view in dome format through your connected projector.
6.  Download the full dome version of the Impacts tour - [http://cdn.worldwidetelescope.org/Content/Planetariums/Impacts%20-%20FULL%20DOME%20v2.1.wtt](http://cdn.worldwidetelescope.org/Content/Planetariums/Impacts%20-%20FULL%20DOME%20v2.1.wtt).
7.  Load and play the tour. Run the tour through once to cache the data. Subsequent viewing should not show data loading.
8.  If performance is choppy take a look at the [Setting Up/Tweaking Performance](/Learn/SettingUp#performance) document.

### Cluster Quick Start

WWT can be setup on multiple computers with a single **master** and 1 or more **projection servers**. You can build your own system from scratch or install WWT alongside an existing planetarium system.

1.  Get the hardware ready.
    1.  Make sure the master computer is setup connected to a desktop monitor and all projection servers (one per projector) are connected to their projectors and that all servers and projectors are powered on.
    2.  Also, make sure the audio output of the master computer is connected to a dome audio system.
    3.  Connect all computers to the network.
2.  Setup the cluster environment. Usually people make a network share that all projection servers can access and put the installer there and then use VNC to login to each computer and do the initial install. Or you can login to each projector server and download from a USB drive or the Internet.
3.  Follow the [Multi-Channel Setup Guide](software_installation.md)
4.  Download the full dome version of the Impacts tour - [http://cdn.worldwidetelescope.org/Content/Planetariums/Impacts%20-%20FULL%20DOME%20v2.1.wtt](http://cdn.worldwidetelescope.org/Content/Planetariums/Impacts%20-%20FULL%20DOME%20v2.1.wtt)
5.  Load the Impacts tour on the Master.
6.  Send the Tour to the projection servers – **Guided Tours/Send Tour to Projection Servers**. Make sure that **Guided Tours/Automatic Tour Sync with Projects Servers** is checked. This will ensure that any changes to the tour on the master are sent immediately to the projection severs.
7.  Load and play the tour. Run the tour through once to cache the data. Subsequent viewing should not show data loading
8.  If performance is choppy take a look at the [Setting Up/Tweaking Performance](http://www.worldwidetelescope.org/Learn/SettingUp#performance) document.

### Making Your Own Dome Shows

You can play any Tour on the dome. Some objects may not be placed in the desired location and timing may require adjustment. Of course you can also create tours from scratch designed specifically for the dome. Details of authoring for the dome are available [here](http://www.worldwidetelescope.org/Learn/Authoring#domeauthoring).
