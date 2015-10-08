# Introduction #

We're still going to deliberate on the plausibility of HD video recording (most likely 720p, since 1080p seems to be a bit lofty).  The video data would have to be compressed on the fly.

The ATSC (Advanced Television Systems Committee) has a set of standards for HD video.  If we want our project to have some legitimacy in this sense, we can try to achieve these standards and call our product ATSC-Compliant (or something).

# Details #

**Progressive or Interlaced**
1080p offers progressive and interlaced framing, the latter of which makes the picture quality higher but makes compression very hard.  720p only offers progressive framing, but that's better anyways, since compression is faster and better.

**Frame Rate**
The ATSC has the following standard frame rate for HD: 24, 25, 30, 60 fps.  We can save a lot of processing power, bandwidth, and space by going down to 24 fps (which is the lowest in the HD standard).  (It's a linear relationship between bandwidth and fps, and between space and fps.  You know what they alway say: "Aim low."  We'll set this as our minimum, and if we think we can go higher, we can.

**Storage**
Uncompressed, 1280x720 @ 24fps is 332 Mbps (Megabits per second), which means about 36 GB for 15 minutes of video.  We could do that with a small portable hard drive or a gigantic flash drive, and compress when the chopper returns.  But I assume we're not; we're going for on-the-fly compression.