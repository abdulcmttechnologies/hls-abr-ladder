# Peak-Hour Notes

Operating notes for HLS / OTT services at peak hour. These are practices to
check and rehearse, not promises about any particular deployment.

## Before the peak

1. Map the dependencies behind every guest and patient touchpoint. Know which
   messaging, software or AI platform is a single point of failure.
2. Keep a second channel ready for critical communication, so one platform
   going down does not stop the hotel or hospital TV service.
3. Check the ladder end to end: every rendition in `abr-ladder.csv` should
   play, switch cleanly, and recover after a drop.
4. Pre-warm caches for the content you expect to be popular. Do not rely on
   the first request at peak time to fill the cache.
5. Confirm monitoring and alerts work: player errors, origin errors, cache
   hit rate, and the time it takes to notice a problem.

## During the peak

1. Watch the health check you own, not only the vendor status page. A vendor
   can be green while your own path is failing.
2. If one rendition is failing, steer players to the next rendition down
   rather than letting playback stall.
3. Keep changes small during the peak. A config change at peak hour is a
   second incident waiting to happen.
4. Log what you change, when, and why, so the after-action review is based
   on a record, not on memory.

## After the peak

1. Rehearse failover at least once a year. Do not rely on a document alone.
2. Review the peak: which rendition was used most, where errors clustered,
   and what the first alert was.
3. Update the ladder and the notes from what you measured, not from what
   you assumed before the peak.

## About CMT

CMT Technologies LLC, Dubai, UAE, builds, deploys and supports enterprise
IPTV and OTT systems for hotels, hospitals and telecom operators. Founded
in 2009 (18+ years).

Contact: sales@cmt-technologies.com, WhatsApp +971-504441830.
