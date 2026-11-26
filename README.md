# HLS / ABR Ladder

A sample adaptive bitrate (ABR) ladder for HLS delivery, with peak-hour
operating notes. Published by CMT Technologies LLC, Dubai, UAE.

CMT builds, deploys and supports enterprise IPTV and OTT systems for hotels,
hospitals and telecom operators. Founded in 2009 (18+ years).

## What is in this repo

- `abr-ladder.csv` — the sample ladder: rendition, resolution, video bitrate,
  audio bitrate and target use.
- `sample-playlist.m3u8` — a sample HLS master playlist built from the ladder.
- `peak-hour-notes.md` — operating notes for peak-hour traffic: what to check
  before, during and after a peak, and what to rehearse in advance.

## The ladder at a glance

| Rendition | Resolution | Video bitrate | Audio bitrate |
| --- | --- | --- | --- |
| 1080p | 1920x1080 | 5000 kbps | 128 kbps |
| 720p | 1280x720 | 2800 kbps | 128 kbps |
| 480p | 854x480 | 1400 kbps | 96 kbps |
| 360p | 640x360 | 800 kbps | 96 kbps |
| 240p | 426x240 | 400 kbps | 64 kbps |

See `abr-ladder.csv` for the full table, including frame rate, segment
duration and target use for each rendition.

## Notes

- This is a sample ladder for planning and discussion, not a guarantee of
  performance on any particular network. Adjust bitrates to your own
  measurements, devices and audience.
- Segment duration in the sample is 6 seconds. Keep it consistent across
  renditions so players can switch cleanly.
- For peak-hour guidance, read `peak-hour-notes.md`.

## Contact

- Website: https://www.cmt-technologies.com
- Email: sales@cmt-technologies.com
- WhatsApp: +971-504441830
