# Explorence

The vision of Explorence was to "bring the video game outside". At this moment in time, GPS-based apps were getting a lot of attention from the press and investors. I had been tinkering with Android for about a year before helping out Explorence with Android late 2010. In early 2011, I was invited to join as co-founder. 

We started with Android early on (2011) because we believed it was gonna breakout. We shifted to iOS due to simple forces: Android was still way behind iOS technology wise, more importantly, iOS owned the mobile startup realm at this moment in time.

```
├── CrittersInc     // an iOS-only title released in 2013
├── Dash            // series of iOS titles released in 2012
│   ├── BullDash    // iOS title released summer 2012
│   ├── DemonDash   // iOS title release october 2012
│   ├── StreetDash  // Android title never released 2011
│   └── TorchDash   // iOS title released summer 2012 
└── links
```

## DASH! - 2010 (Android)

DASH! on Android was the starting point for Explorence's GPS-based games, and was the first iteration of the Dash series of titles.  If the UI looks bad it's because I made it, and we didn't have a designer yet :) Also, most Android apps looked bad compared to iOS apps at this time. [DASH! demo with the Scobelizer](https://www.youtube.com/watch?v=3-mdcn_YM6U) .

#### Screencaps

<p float="left">
  <img src="./links/scobelizer_screencaps/DASH_homescreen.png" width="128" />
  <img src="./links/scobelizer_screencaps/DASH_challengelist.png" width="128" /> 
  <img src="./links/scobelizer_screencaps/DASH_challengedetails.png" width="128" />
    <img src="./links/scobelizer_screencaps/DASH_mapview.png" width="128" />
</p>

#### Live demo screen caps from Scobelizer interview

<p float="left">
  <img src="./links/scobelizer_screencaps/DASH_demo_01_homescreen.png" width="128" />
  <img src="./links/scobelizer_screencaps/DASH_demo_01_homescreen.png" width="128" />
  <img src="./links/scobelizer_screencaps/DASH_demo_01_homescreen.png" width="128" />
  <img src="./links/scobelizer_screencaps/DASH_demo_01_homescreen.png" width="128" />
  <img src="./links/scobelizer_screencaps/DASH_demo_01_homescreen.png" width="128" />
  <img src="./links/scobelizer_screencaps/DASH_demo_01_homescreen.png" width="128" />
</p>

A core feature of DASH! was using GPS to create "challenges", and then allow the user to share a GPS track with friends. To get the GPS tracking off the ground, we pretty much hacked the open source Android project [MyTracks](https://en.wikipedia.org/wiki/MyTracks). The GPS data was stored in the GPX format locally on the Android device, and then shared to our server.
## StreetDash - 2011 (Android)

The second iteration of DASH! was StreetDash. It had a much better UI due to the fact we brought on an artist to help with UI. (This may have been released on the Google Play Store but I can't remember, if it was released, it wasn't live very long).

#### Mockup and flow

<p float="left">
  <img src="./Dash/StreetDash/streetdash_flow.png" width="512" />
</p>

#### App screenshots

<p float="left">
  <img src="./Dash/StreetDash/AppStoreScreenshots/IMG_0076.PNG" width="128" />
  <img src="./Dash/StreetDash/AppStoreScreenshots/IMG_0077.PNG" width="128" />
  <img src="./Dash/StreetDash/AppStoreScreenshots/IMG_0079.PNG" width="128" />
  <img src="./Dash/StreetDash/AppStoreScreenshots/IMG_0080.PNG" width="128" />
  <img src="./Dash/StreetDash/AppStoreScreenshots/IMG_0095.PNG" width="128" />
</p> 

## Dash 2012 titles (iOS)
The summer of 2012 was unique because the Running of the Bulls in Pamplona, Spain coincided with the 2012 Summer Olympics. We tried to capitalize on this by releasing BullDash, and then TorchDash. 

#### About our backend

A co-founder left for greener pastures, and I took over backend development. I inherited a code base built on Groovy on Grails, backed by MySQL, sending XML over the wire, deployed to Elastic Beanstalk on AWS. NOTE: I had zero experience coding and deploying a web server. 
<p>
The GPS track data recorded on a user's Android or iOS device was shared over the wire in the [GPX format](https://en.wikipedia.org/wiki/GPS_Exchange_Format). I migrated our API to JSON, but let the GPX implementation remain, mostly because refactoring that out of the database did not make sense. 
</p>

<p>
A final note on the backend. It was not architected with **multitenancy** in mind. 
At that time, I had no idea that this sort of architecture existed.  The follwing three apps were supported by cloning the code base to support each game (lesson learned). 
</p>

### BullDash - 2012 (iOS)
#### Mockup and flow

<p float="left">
  <img src="./Dash/BullDash/mockups/bulldash_flow.png" width="512" />
</p>

#### App screenshots

<p float="left">
  <img src="./Dash/BullDash/Screenshots/IMG_0174.PNG" width="128" />
  <img src="./Dash/BullDash/Screenshots/tutorial.png" width="128" />
  <img src="./Dash/BullDash/Screenshots/photo_9.PNG" width="128" />
  <img src="./Dash/BullDash/Screenshots/IMG_0178.PNG" width="128" />
  <img src="./Dash/BullDash/Screenshots/IMG_0193.PNG" width="128" />
  <img src="./Dash/BullDash/Screenshots/IMG_0179.PNG" width="128" />
  <img src="./Dash/BullDash/Screenshots/IMG_0192.PNG" width="128" />
  <img src="./Dash/BullDash/Screenshots/career.PNG" width="128" />
</p> 

### TorchDash -2012 (iOS)

TorchDash was released to coincide with the 2012 Summer Olympics and the artistic inspiration was classic Greek. 
#### Mockup and flow

<p float="left">
  <img src="./Dash/TorchDash/torchdash_flow.png" width="512" />
</p>

#### App screenshots

<p float="left">
  <img src="./Dash/TorchDash/mockups/fb_login.png" width="128" />
  <img src="./Dash/TorchDash/mockups/homescreen.png" width="128" />
  <img src="./Dash/TorchDash/mockups/friend_list.png" width="128" />
  <img src="./Dash/TorchDash/mockups/pre-race.png" width="128" />
  <img src="./Dash/TorchDash/mockups/challenge0.png" width="128" />
  <img src="./Dash/TorchDash/mockups/challenge1.png" width="128" />
  <img src="./Dash/TorchDash/mockups/challenge2.png" width="128" />

  <img src="./Dash/TorchDash/mockups/career.png" width="128" />
</p> 

### DemonDash - 2012 (iOS)

DemonDash was a zombie/demon inspired app, released around Halloween 2012. 

#### Mockup and flow

<p float="left">
  <img src="./Dash/DemonDash/pumpkin_flow.jpg" width="512" />
</p>
#### App screenshots

<p float="left">
  <img src="./Dash/DemonDash/iphone_screenshots/iphone5_home.png" width="128" />
  <img src="./Dash/DemonDash/iphone_screenshots/iphone5_mummies.png" width="128" />
  <img src="./Dash/DemonDash/iphone_screenshots/iphone5_witches.png" width="128" />
  <img src="./Dash/DemonDash/iphone_screenshots/iphone5_win.png" width="128" />
</p> 

## Critters Inc.

WIP