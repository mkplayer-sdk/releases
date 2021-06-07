---
# Mediakind WMC SDK Releases

## Quick Release Links: [NPM Repository](https://www.npmjs.com/package/@mediakind/wmc) | [Reference Doc](https://wmc.mr.tv3cloud.com/nba/docs/index.html) | [RefApp Link](https://wmc.mr.tv3cloud.com/nba/refapp/index.html)

## Release - 1.40.11
- Improvements:
    -  Added support for HLS+WV and HLS+PR Encrypted Playback on Chrome and Edge browsers
    -  Added Xbox encrypted playback support
    -  Removed debugger lock from release/secure builds and NPM releases
    -  Added accountId in ....
    -  Improve WMC-SDK documentation
       - Added an example tutorial for encrypted playback of MK assets
       - Added player key and domain white- list related information
       - Updated with MKP service related communication API

- Bug Fixes:
    -  


## Release - 1.40.10
- Bug Fixes:
    -  Bug 1237812: On performing restart operation, VOD asset throws '4-44-225' error
 - Improvements:
    -  PBI 1238049: Implement Restart Window PBR
    -  Improve WMC-SDK documents
## Release - 1.40.9
- Bug Fixes:
    -  Bug 1242738: CDN selection issue when multiple CDN assign from backend
 - Improvements:
    -  WMC SDK to handle playback control blocking PBRs during Program Change.
## Release - 1.40.8
- Bug Fixes:
    - Bug 1203880: After the Quality levels change, Paused media is getting Resumed
 - Improvements:
    -  Improve WMC-SDK documents.
## Release - 1.40.7
 - Bug Fixes:
    - Bug 1238223: Enable Live manifest by default and remove RefApp UI interface for feature
    - Bug 1238047: Program timer is not getting updated on player screen, although the query is coming properly
    - Bug 1227021: 4-44-2413 - Reached the max parallel limit
 - Improvements:
    -  PBI 1232680: WMC SDK to handle playback control blocking PBR's.
## Release - 1.40.6
 - Bug Fixes:
   - Bug 1231979: [WMC][Safari][Live manifest] Manifest changes from start=<LIVE> to start=<SlotStartTime> after performing one skip rewind
 - Improvements:
    - PBI 1232682: [NBA] CDN selection should be based on priority and cdnFailoverPercent
    - PBI 1232683: [NBA] CDN Tokenisation handling
    - PBI 1232679: [NBA][P1] WMC SDK to handle Playback blocking PBR's
