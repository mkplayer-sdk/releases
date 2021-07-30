# MKPlayerSDK Android Releases

Quick Links: [MKPlayer Artifactory Repo](https://mkplayer.jfrog.io/ui/repos/tree/General/mkplayer%2Fcom%2Fmediakind%2Fmkplayer)
## 1.0.4 - 2021.07.30
Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/android/docs/1.0.4/) | [Android Reference App](https://mkplayer.z13.web.core.windows.net/android/refapp/MKPlayer-RefApp-Android-1.0.4.zip)
**Added:**
- Added support for Closed captions
- Added SessionId in User Information passed to PRISMA
## 1.0.3 - 2021.07.16
Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/android/docs/1.0.3/) | [Android Reference App](https://mkplayer.z13.web.core.windows.net/android/refapp/MKPlayer-RefApp-Android-1.0.3.zip)

**Added:**
- Added support for Picture in Picture

## 1.0.2 - 2021.07.02
Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/android/docs/1.0.2/) | [Android Reference App](https://mkplayer.z13.web.core.windows.net/android/refapp/MKPlayer-RefApp-Android-1.0.2.zip)

**Added:**
- Added support for Seeking within the live manifest
   - Added getSeekableRange API to allow the user to query the current seekable range that is  valid in the live window
- Added support to append personalInfo params to the manifest URL
- Added support to override the existing key/values in the manifest URL with the CDN token


## 1.0.1 - 2021.06.18
Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/android/docs/1.0.1/) | [Android Reference App](https://mkplayer.z13.web.core.windows.net/android/refapp/MKPlayer-RefApp-Android-1.0.1.zip)

**Added:**
- Efficient thread synchronisation in abrupt scenarios

**Fixed:**
- Fixed app crash after invoking player.onActivityDestroyed() while playback is initiated


## 1.0.0 - 2021.06.08
Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/android/docs/1.0.0/) | [Android Reference App](https://mkplayer.z13.web.core.windows.net/android/refapp/MKPlayer-RefApp-Android-1.0.0.zip)

**Added:**
- Program Query for Live channels
- Playback Restriction (PBR) support for Live across program boundary transition
- Provided Video Scaling mode APIs from SDK 
- Added accoundId to MKPBackendConfiguration
- Added API updateAuthToken() to provide means to update the auth token during playback
- Support for playback using JWT based auth token

**Changed:**
- Bitmovin player version upgraded to 2.66.0
- Renamed MKPSourceConfiguration param applicationName to applicationToken

**Deprecated:**
- Previous MKPBackendConfiguration constructor is deprecated. Refer to 1.0.0 doc for updated constructor.
- Previous MKPSourceConfiguration constructor is deprecated. Refer to 1.0.0 doc for updated constructor.

**Fixed:**
- Handled NPE from load method if mandatory params of MKPBackendConfiguration are missing


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
