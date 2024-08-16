# senseiplay_HD

This is a release of Senseiplay from digarok of NinjaForce which adds a vidHD text mode visualizer for playback.  It also includes a small collection of MODs suited to this visualizer, or just for listening to!
![IMG_0435](https://github.com/user-attachments/assets/6e080baa-c49a-405b-a8ed-0c87f8ae85ea)
KansasFest 2024 video: https://youtu.be/8otShYbtIkk
## System Requirements

System Requirements:
  
    - Apple IIgs with 1 MB of RAM (more if you want to load gigantic MODs)
    - vidHD card (fw 1.15) in any supported slot for
      your ROM (Slot 1-6 for ROM 3, Slot 3 for ROM 01)
      Set to Your Card if not in Slot 3
    
Recommended:

    - Stereo Card 
    - Zip GSX or TranswarpGS (does not make a huge difference though)
      AppleSqueezer can work but is less stable, perhaps due to DMA incomopatibilities
    - Those new, small OLED HDMI displays look amazing with the visualizer


## How do i...

You can just mount and boot the disk image, or launch it from ProDOS BYE.
If you don't have a vidHD card in your Apple IIGS, SenseiPlay works pretty much like the original.
If you do, you're going to want to either
1) Enable Keyboard Buffering in your IIGS Control Panel or
2) Go into the vidHD control panel and set the Resolution to 120 x 67. (this is also required for AppleSqueezer to work).

Keyboard Buffering allows a hack/trick that uses the ADB keyboard buffer to press "ESC 2" to enable the mid resolution vidHD text mode.

From there, you can just navigate to the MUSIC folder or your folder of NinjaTracker Plus music to play them.  If you have a vidHD, the "V" option is enabled at launch.  You can always disable it during or between plays by pressing "V".

The Command key gives a short (but not comprehensive) list of key commands - but most of these are for debug purposes so YMMV.  Definitely have fun with the K key to initiate the snake or the T key to force a constellation/shape to be formed, or any combination of the two.  And the M key switches to the piano view which gives a nice perspective on the notes the NTP MOD is playing (and arpeggios look really cool and fast).  The effects column in this mode is unfinished.

## How does it work?

The vidHD text modes were originally intended as a way to get a higher resolution program listing, or maybe for someone to make a terminal program.  As a result they were not designed for performance or fast animation.  They use the COUT and Pascal text protocols and the standard 80 column terminal functions, and are only fast enough for a few dozen character plots per 1/60th of a second frame.  However, there *are*  a few terminal commands that allow affecting large portions of the screen with a single character command.  Thus it's possible to create very fast 60 FPS "VU meters" using only a few plots.  The rest of the plots are used for drawing the stars and moving them around.  The end result is a decent number of things moving around despite the low "plots per second".

## What's next?

I'd like to add some more visual modes as time and know-how strikes.  The original vidHD is essentially out of production, but there are quite a few new video solutions that could support similar extended text modes.  Hopefully they will.  There may also be a vidHD 2 in the near future.  I would definitely be interested in updating the visualizer to support newer cards with hopefully more performance for plotting!


## Download

Grab it from the release page: https://github.com/01craft/senseiplay_HD/releases/download/v0.96/senseiplayhd.po


## The Original SenseiPlay?

This app is based on SenseiPlay https://github.com/digarok/senseiplay, however merging the code has not yet happened due to time, etc, so we agreed I would just host a separate binary for the time being.
