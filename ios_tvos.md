
# MKPlayerSDK iOS/tvOS Releases

## 1.0.1 (2021.07.02)

Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/ios_tvos/docs/1.0.1/) | [iOS Reference App](https://mkplayer.z13.web.core.windows.net/ios_tvos/refapp/MKPlayer-RefApp-iOS-1.0.1.zip) | [tvOS Reference App](https://mkplayer.z13.web.core.windows.net/ios_tvos/refapp/MKPlayer-RefApp-tvOS-1.0.1.zip)

**Added:**
- Added support for Seeking within the live manifest
- Exposed getSeekableRange() API to allow user to seek within the live window
- Added support to append personalInfo params to the manifest URL
- Added support for the key/values in the CDN Token to overwrite with the matching key/values in the manifest URL and append the key/values if do not exist
- Printing the live latency in the RefApp


## 1.0.0 (2021.06.08)

Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/ios_tvos/docs/1.0.0/) | [iOS Reference App](https://mkplayer.z13.web.core.windows.net/ios_tvos/refapp/MKPlayer-RefApp-iOS-1.0.0.zip) | [tvOS Reference App](https://mkplayer.z13.web.core.windows.net/ios_tvos/refapp/MKPlayer-RefApp-tvOS-1.0.0.zip)

**Added:**
- Provided Video Scaling mode APIs from SDK
- Added accoundId to MKPBackendConfiguration
- Added API updateAuthToken() to provide means to update the auth token during playback
- Support for playback using JWT based auth token

**Changed:**
- Bitmovin player version upgraded to 2.64.0
- Renamed MKPSourceConfiguration param applicationName to applicationToken


## 0.9.9 (2021.05.21)

Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/ios_tvos/docs/0.9.9/) | [iOS Reference App](https://mkplayer.z13.web.core.windows.net/ios_tvos/refapp/MKPlayer-RefApp-iOS-0.9.9.zip) | [tvOS Reference App](https://mkplayer.z13.web.core.windows.net/ios_tvos/refapp/MKPlayer-RefApp-tvOS-0.9.9.zip)

**Change log:**
- Improvements to PBR support for Live across program boundary transition
- Improvements to RefApp UI for tvOS
   - Implemented the draggable progress bar for the seek functionality
   - Focus issue with restart button - Fixed
   - Selecting subtitle and audio track was not working properly due to focus issue - Fixed
   - Swipe up is not hiding the subtitle and audio track view - Fixed
   - 10 sec seek button takes time to hide - Fixed


## 0.9.8 (2021.05.07)

Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/ios_tvos/docs/0.9.8/) | [iOS Reference App](https://mkplayer.z13.web.core.windows.net/ios_tvos/refapp/MKPlayer-RefApp-iOS-0.9.8.zip) | [tvOS Reference App](https://mkplayer.z13.web.core.windows.net/ios_tvos/refapp/MKPlayer-RefApp-tvOS-0.9.8.zip)

**Change log:**
- Added playback restriction (PBR) support
   - Support added for playback blocking PBRs for Jailbroken devices and extended display over HDMI dongle (enforced at the App level - Ex: RefApp).
   - Support added for checking playback restrictions for Live services on tune and across program boundary.
   - Support for stream count based restrictions.
   - Not supported PBR - Out-of-Home blocked
- [MKPErrorEvent](https://mkplayer.z13.web.core.windows.net/ios_tvos/docs/0.9.8/Classes/MKPErrorEvent.html) properties `errorCode` and `errorMessage` now renamed to `code` and `message` respectively.
- Xcode 12.5 support.

**Note:** You will need to update your Xcode version to 12.5 to use this release. v0.9.8 is no longer compatible with earlier versions of Xcode.


## 0.9.7 (2021.04.23)

Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/ios_tvos/docs/0.9.7/) | [iOS Reference App](https://mkplayer.z13.web.core.windows.net/ios_tvos/refapp/MKPlayer-RefApp-iOS-0.9.7.zip) | [tvOS Reference App](https://mkplayer.z13.web.core.windows.net/ios_tvos/refapp/MKPlayer-RefApp-tvOS-0.9.7.zip)

**Change log:**
- Added playback restriction (PBR) support
   - Support added for playback blocking PBRs (wifi, cellular, Airplay, phone, tablet, iOS blocked PBRs)   
   - Support added for playback control blocking PBRs (rewind, fastForward, seekBackward, seekForwards, pause/resume, restart blocked PBRs)
   - Not supported PBRs - Program boundary scenario for Live, Stream count, Jail broken, HDMI blocked, AV Adapter, OOH blocked
- Shortcode Authentication for RefApp
- Ability to pass CDN token in master manifest URL
- Added support for CDN selection based on cdnFailoverPercent 


## 0.9.6 (2021.04.09)

Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/ios_tvos/docs/0.9.6/) | [iOS Reference App](https://mkplayer.z13.web.core.windows.net/ios_tvos/refapp/MKPlayer-RefApp-iOS-0.9.6.zip) | [tvOS Reference App](https://mkplayer.z13.web.core.windows.net/ios_tvos/refapp/MKPlayer-RefApp-tvOS-0.9.6.zip)

**Change log:**
- Bitmovin Analytics integrated on tvOS


## 0.9.5 (2021.03.27)

Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/ios_tvos/docs/0.9.5/) | [iOS Reference App](https://mkplayer.z13.web.core.windows.net/ios_tvos/refapp/MKPlayer-RefApp-iOS-0.9.5.zip) | [tvOS Reference App](https://mkplayer.z13.web.core.windows.net/ios_tvos/refapp/MKPlayer-RefApp-tvOS-0.9.5.zip)

**Change log:**
- Bitmovin Analytics Integrated
- Enabled Airplay support
- Support for Buffer controls
- Support for SourceOptions
- Support for full screen on changing orientation
- Deprecated DeveloperID for UMCless communication

Known Issues: 
- Bitmovin analytics not integrated in tvOS


## 0.9.3 (2021.03.09)

Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/ios_tvos/docs/0.9.3/) | [iOS Reference App](https://mkplayer.z13.web.core.windows.net/ios_tvos/refapp/MKPlayer-RefApp-iOS-0.9.3.zip) | [tvOS Reference App](https://mkplayer.z13.web.core.windows.net/ios_tvos/refapp/MKPlayer-RefApp-tvOS-0.9.3.zip)

**Change log:**
- Live and VOD clear and encrypted content playback support 
- Multiple audio and subtitles support
- Support for playback controls like Pause/Resume, Restart (play from beginning), Skip back 10 seconds, Skip forwards 10 seconds
- Basic RefApp available to validate the VOD/Live playback
- Bitcode support for iOS/tvOS

Known Issues: 
- DAI Support for HLS (Not available yet)

## 0.9.2 (2021.02.25)
Links: [Reference Doc](https://mkplayer.z13.web.core.windows.net/ios_tvos/docs/0.9.2/) 
- Initial release.
