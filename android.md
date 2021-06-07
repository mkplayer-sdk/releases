# MKPlayerSDK Android Releases

Quick Links: [MKPlayer Artifactory Repo](https://mkplayer.jfrog.io/ui/packages)

## 1.0.0 - 2021.06.07
Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/android/docs/1.0.0/) | [Android Reference App](https://mkplayer.z13.web.core.windows.net/android/refapp/MKPlayer-RefApp-Android-1.0.0.zip)

**Change log:**

**Added:**
- Program Query for Live channels
- Playback Restriction (PBR) support for Live across program boundary transition
- Provided Video Scaling mode APIs from SDK 
- Pass accountId for MKPBackendConfiguration to support guest user epic changes...??
- STS token update during playback ??

**Changed:**
- Bitmovin player version upgraded to 2.66.0

**Deprecated:**
- Previous MKPBackendConfiguration constructor is deprecated. Refer 1.0.0 doc for updated constructor.
- Previous MKPSourceConfiguration constructor is deprecated. Refer 1.0.0 doc for updated constructor.

**Fixed:**
- Handled NPE from load method if mandatory params of MKPBackendConfiguration is missing

**Known Issues:**



## 0.9.8 - 2021.05.07
Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/android/docs/0.9.8/) | [Android Reference App](https://mkplayer.z13.web.core.windows.net/android/refapp/MKPlayer-RefApp-Android-0.9.8.zip)

**Change log:**
- Added playback restriction (PBR) support
   - Support added for playback blocking PBR for extended display via HDMI dongle (enforced at the app level - Ex: RefApp)
   - Support for stream count based restrictions.
   - Not supported PBR - Program boundary scenario for Live, Rooted device restrictions, Out-of-Home blocked
- Support for Short-Code-Authentication to refresh the STS token in the RefApp.


## 0.9.7 - 2021.04.23
Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/android/docs/0.9.7/) | [Android Reference App](https://mkplayer.z13.web.core.windows.net/android/refapp/MKPlayer-RefApp-Android-0.9.7.zip)

**Change log:**
- Added playback restriction (PBR) support
   - Support added for playback blocking PBRs (wifi, cellular, phone, tablet blocked pbrs)
   - Support added for playback control blocking PBRs (rewind, fastForward, seekBackward, seekForwards, pause/resume, restart blocked pbrs)
   - Not supported PBR - Program boundary scenario for Live, Stream count, Jail broken, HDMI blocked, AV Adapter, OOH blocked
- Ability to pass CDN token in master manifest URL
- Added support for CDN selection based on cdnFailoverPercent
- HLS + WV playback support on Android devices 


## 0.9.4 - 2021.04.09
Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/android/docs/0.9.4/) | [Android Reference App](https://mkplayer.z13.web.core.windows.net/android/refapp/MKPlayer-RefApp-Android-0.9.4.zip)

**Change log:**
- Optimised Android RefApp for FireTV support
  - Added Leanback support
  - Designed new UI to support FireTV
  - Handled remote key events
- Bitmovin version updated to 2.64.0 to fix missing metadata events for DAI



## 0.9.3 - 2021.03.26
Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/android/docs/0.9.3/) | [Android Reference App](https://mkplayer.z13.web.core.windows.net/android/refapp/MKPlayer-RefApp-Android-0.9.3.zip)

**Change log:**
- Bitmovin Analytics Integrated
- Support for selectable quality controls, Adaptation, Buffer controls
- Support for SourceOptions
- Support for wake lock and full screen
- Deprecated use of initPlayer(). MKPlayer construction takes care of initialization
- Deprecated DeveloperID for UMCless communication




## 0.9.2 - 2021.03.08
Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/android/docs/0.9.2/) | [Android Reference App](https://mkplayer.z13.web.core.windows.net/android/refapp/MKPlayer-RefApp-Android-0.9.2.zip)

**Change log:**
- Live and VOD clear and encrypted content playback support 
- Multiple audio and subtitles support
- Support for playback controls like Pause/Resume, Restart (play from beginning), Skip back 10 seconds, Skip forwards 10 seconds
- Basic RefApp available to validate the VOD/Live playback
- Dynamic Ad Insertion support
  - Support for Single/Multiple Ad in single Ad slot
  - RefApp: Displaying Ad Quartile events indicating the percentage of Ad being played

Known Issues:
- RefApp: DAI Ad markers not available yet 

## 0.9.1 - 2021.03.03
Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/android/docs/0.9.1/) 
- Initial release.
