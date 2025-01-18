# Bass Arena Expansion

A mod that adds 10 new tracks to the Bass Arena Radio in Forza Horizon 5.
(Please note that in order to add these tracks, it replaces 10 tracks in the XS Radio which will have 12 tracks instead of 22)

### New Tracks List:
- [Armin Van Buuren, David Guetta, Aldae - In The Dark](https://music.youtube.com/watch?v=vh0IbMVKgaI)
- [Calvin Harris - Feel So Close](https://music.youtube.com/watch?v=Nh_bdvA8cVM)
- [Calvin Harris - My Way](https://music.youtube.com/watch?v=aTEa2CgmsMA)
- [Jason Ross, Dia Frampton - Take You Home](https://music.youtube.com/watch?v=Q8PQkVo99pk)
- [Kygo, Justin Jesso - Stargazing](https://music.youtube.com/watch?v=UrJRHUhAQNA)
- [Martin Garrix - Animals](https://music.youtube.com/watch?v=DYf28lOb8KU) *For Asphalt 8 nostalgics*
- [Martin Garrix, Matisse, Sadko - Forever](https://music.youtube.com/watch?v=fSQ85nHRXw8)
- [Martin Garrix - Won't Let You Go](https://music.youtube.com/watch?v=oaMxA5-z1jo)
- [Noisestorm - Crab Rave](https://music.youtube.com/watch?v=c_sNBS-9Ras)
- [R3HAB - Loca Loca (Vion Konger Remix)](https://music.youtube.com/watch?v=a67LRVpkARo)

## You can download this [mod hehe](https://drive.usercontent.google.com/download?id=157ahCs2rC0ZlbdO5RhCkZGKOQx5TODft)

## Installation Guide

**Note:** This mod was originally made for FH5 version [1.634.818.0](https://support.forzamotorsport.net/hc/en-us/articles/25987415101843-FH5-Release-Notes-February-6th-2024-Hotfix). Therefore, all new tracks added after this version will not be included.

In order to follow this guide, you should find the location of your Forza Horizon 5 folder (which contains all the files of the game).

**Important:** Please create a copy of the following files to avoid having to reinstall the game in the event of a problem or if you wish to uninstall the mod at a later date:
- Forza Horizon 5/media/Audio/``RadioInfo_YourLanguage.xml`` (e.g., RadioInfo_FR.xml)
- Forza Horizon 5/media/Audio/FMODBanks/``R4_Tracks_CU1.assets.bank``
- Forza Horizon 5/media/Audio/FMODBanks/``R4_Tracks_CU1.bank``

This should work on Steam and Windows Store version.

### Step 1: Replacing Bank File(s)
- Replace the ``R4_Tracks_CU1.assets.bank`` with the new ``R4_Tracks_CU1.assets.bank`` (which should be located in YourGamePath/Forza Horizon 5/media/Audio/FMODBanks/ folder).

- If you're not in version [1.634.818.0](https://support.forzamotorsport.net/hc/en-us/articles/25987415101843-FH5-Release-Notes-February-6th-2024-Hotfix), you should probably replace the ``R4_Tracks_CU1.bank`` with the ``R4_Tracks_CU1.bank`` from v1.634.818.0.

### Step 2: Editing the RadioInfo_YourLanguage.xml File
- Add this line ``<Bank Name="R4_Tracks_CU1" />`` to the bank list. You should have something
```XML
...
<RadioStation Name="Horizon Bass Arena" Number="2">
      <MediaTrackRestrictions />
      <Banks>
        <Bank Name="R2_Tracks_Disk" />
        <Bank Name="R2_Tracks_CU1" />
        <Bank Name="R2_Tracks_CU2" />
        <Bank Name="R4_Tracks_CU1" />
        <Bank Name="R2_Tracks_PDLC1" />
        <Bank Name="R2_LFE" />
        <Bank Name="R2_Stingers_FR" />
        <Bank Name="R2_Stingers_LFE" />
        <Bank Name="VO_DJ_02_FR" />
        <Bank Name="VO_PDLC1_DJ_02_FR" />
        <Bank Name="VO_PDLC2_DJ_02_FR" />
      </Banks>
...
```

- Add the new tracks in the Sample List (``<SampleList Type="Track" Event="/Master/Radio/Track"></SampleList>`` section in the Bass Arena Radio section):
```xml
...
        <Sample SoundName="HZ5_R4_AngelicaGarcia_KarmaTheKnife" SampleLength="7768064" SampleRate="48000" DisplayName="Animals" Artist="Martin Garrix" IsXCloudModeSafe="true">
          <Marker Name="VeryStart" Position="-1" />
          <Marker Name="TrackStart" Position="0" />
          <Marker Name="DJDrop" Position="871242" />
          <Marker Name="TrackDrop" Position="1565798" />
          <Marker Name="TrackLoopStart" Position="2510151" />
          <Marker Name="TrackLoopEnd" Position="6125001" />
          <Marker Name="DJSegment" Position="3227644" />
          <Marker Name="PostDrop" Position="3227644" />
          <Marker Name="PostRaceLoopStart" Position="4216431" />
          <Marker Name="PostRaceLoopEnd" Position="4856836" />
          <Marker Name="StingerStart" Position="7684868" />
          <Marker Name="DJStart" Position="7685868" />
          <Marker Name="End" Position="7768064" />
          <Marker Name="Loop1Start" Position="-1" />
          <Marker Name="Loop1End" Position="-1" />
          <Marker Name="Loop2Start" Position="-1" />
          <Marker Name="Loop2End" Position="-1" />
          <Marker Name="Loop3Start" Position="-1" />
          <Marker Name="Loop3End" Position="-1" />
          <Marker Name="Loop4Start" Position="-1" />
          <Marker Name="Loop4End" Position="-1" />
          <Marker Name="Loop5Start" Position="-1" />
          <Marker Name="Loop5End" Position="-1" />
          <Marker Name="Section1" Position="-1" />
          <Marker Name="Section2" Position="-1" />
          <Marker Name="Section3" Position="-1" />
          <Marker Name="Section4" Position="-1" />
          <Marker Name="Section5" Position="-1" />
          <Loop Name="TrackMain" StartMarker="TrackLoopStart" EndMarker="TrackLoopEnd" />
          <Loop Name="TrackPostRace" StartMarker="PostRaceLoopStart" EndMarker="PostRaceLoopEnd" />
          <Loop Name="Loop1" StartMarker="Loop1Start" EndMarker="Loop1End" />
          <Loop Name="Loop2" StartMarker="Loop2Start" EndMarker="Loop2End" />
          <Loop Name="Loop3" StartMarker="Loop3Start" EndMarker="Loop3End" />
          <Loop Name="Loop4" StartMarker="Loop4Start" EndMarker="Loop4End" />
          <Loop Name="Loop5" StartMarker="Loop5Start" EndMarker="Loop5End" />
          <BPM Value="159.8716" Start="81463" />
          <BPM Value="159.8716" Start="11754831" />
        </Sample>
        <Sample SoundName="HZ5_R4_BiteTheBuffalo_Getaway" SampleLength="9225680" SampleRate="48000" DisplayName="My Way" Artist="Calvin Harris" IsXCloudModeSafe="true">
          <Marker Name="VeryStart" Position="-1" />
          <Marker Name="TrackStart" Position="0" />
          <Marker Name="DJDrop" Position="0" />
          <Marker Name="TrackDrop" Position="1369188" />
          <Marker Name="TrackLoopStart" Position="2005480" />
          <Marker Name="TrackLoopEnd" Position="5541607" />
          <Marker Name="DJSegment" Position="4215657" />
          <Marker Name="PostDrop" Position="7758831" />
          <Marker Name="PostRaceLoopStart" Position="8509944" />
          <Marker Name="PostRaceLoopEnd" Position="8862338" />
          <Marker Name="StingerStart" Position="9186573" />
          <Marker Name="DJStart" Position="9187573" />
          <Marker Name="End" Position="9225680" />
          <Marker Name="Loop1Start" Position="-1" />
          <Marker Name="Loop1End" Position="-1" />
          <Marker Name="Loop2Start" Position="-1" />
          <Marker Name="Loop2End" Position="-1" />
          <Marker Name="Loop3Start" Position="-1" />
          <Marker Name="Loop3End" Position="-1" />
          <Marker Name="Loop4Start" Position="-1" />
          <Marker Name="Loop4End" Position="-1" />
          <Marker Name="Loop5Start" Position="-1" />
          <Marker Name="Loop5End" Position="-1" />
          <Marker Name="Section1" Position="-1" />
          <Marker Name="Section2" Position="-1" />
          <Marker Name="Section3" Position="-1" />
          <Marker Name="Section4" Position="-1" />
          <Marker Name="Section5" Position="-1" />
          <Loop Name="TrackMain" StartMarker="TrackLoopStart" EndMarker="TrackLoopEnd" />
          <Loop Name="TrackPostRace" StartMarker="PostRaceLoopStart" EndMarker="PostRaceLoopEnd" />
          <Loop Name="Loop1" StartMarker="Loop1Start" EndMarker="Loop1End" />
          <Loop Name="Loop2" StartMarker="Loop2Start" EndMarker="Loop2End" />
          <Loop Name="Loop3" StartMarker="Loop3Start" EndMarker="Loop3End" />
          <Loop Name="Loop4" StartMarker="Loop4Start" EndMarker="Loop4End" />
          <Loop Name="Loop5" StartMarker="Loop5Start" EndMarker="Loop5End" />
          <BPM Value="108.0035" Start="43871" />
          <BPM Value="108.0035" Start="4577057" />
          <BPM Value="108.0035" Start="6203670" />
        </Sample>
        <Sample SoundName="HZ5_R4_DeathValleyGirls_10DayMiracleChallenge" SampleLength="9168896" SampleRate="48000" DisplayName="Feel So Close" Artist="Calvin Harris" IsXCloudModeSafe="true">
          <Marker Name="VeryStart" Position="-1" />
          <Marker Name="TrackStart" Position="0" />
          <Marker Name="DJDrop" Position="45765" />
          <Marker Name="TrackDrop" Position="2023033" />
          <Marker Name="TrackLoopStart" Position="3022098" />
          <Marker Name="TrackLoopEnd" Position="5668311" />
          <Marker Name="DJSegment" Position="4675167" />
          <Marker Name="PostDrop" Position="7314325" />
          <Marker Name="PostRaceLoopStart" Position="8312721" />
          <Marker Name="PostRaceLoopEnd" Position="8643616" />
          <Marker Name="StingerStart" Position="8950572" />
          <Marker Name="DJStart" Position="8951572" />
          <Marker Name="End" Position="9168896" />
          <Marker Name="Loop1Start" Position="-1" />
          <Marker Name="Loop1End" Position="-1" />
          <Marker Name="Loop2Start" Position="-1" />
          <Marker Name="Loop2End" Position="-1" />
          <Marker Name="Loop3Start" Position="-1" />
          <Marker Name="Loop3End" Position="-1" />
          <Marker Name="Loop4Start" Position="-1" />
          <Marker Name="Loop4End" Position="-1" />
          <Marker Name="Loop5Start" Position="-1" />
          <Marker Name="Loop5End" Position="-1" />
          <Marker Name="Section1" Position="-1" />
          <Marker Name="Section2" Position="-1" />
          <Marker Name="Section3" Position="-1" />
          <Marker Name="Section4" Position="-1" />
          <Marker Name="Section5" Position="-1" />
          <Loop Name="TrackMain" StartMarker="TrackLoopStart" EndMarker="TrackLoopEnd" />
          <Loop Name="TrackPostRace" StartMarker="PostRaceLoopStart" EndMarker="PostRaceLoopEnd" />
          <Loop Name="Loop1" StartMarker="Loop1Start" EndMarker="Loop1End" />
          <Loop Name="Loop2" StartMarker="Loop2Start" EndMarker="Loop2End" />
          <Loop Name="Loop3" StartMarker="Loop3Start" EndMarker="Loop3End" />
          <Loop Name="Loop4" StartMarker="Loop4Start" EndMarker="Loop4End" />
          <Loop Name="Loop5" StartMarker="Loop5Start" EndMarker="Loop5End" />
          <BPM Value="155.8666" Start="77638" />
          <BPM Value="155.8666" Start="7320756" />
        </Sample>
        <Sample SoundName="HZ5_R4_ElShirota_LaCiudad" SampleLength="9633792" SampleRate="48000" DisplayName="Forever" Artist="Martin Garrix, Matisse, Sadko" IsXCloudModeSafe="true">
          <Marker Name="VeryStart" Position="-1" />
          <Marker Name="TrackStart" Position="0" />
          <Marker Name="DJDrop" Position="642253" />
          <Marker Name="TrackDrop" Position="2652126" />
          <Marker Name="TrackLoopStart" Position="2652126" />
          <Marker Name="TrackLoopEnd" Position="7442577" />
          <Marker Name="DJSegment" Position="4110418" />
          <Marker Name="PostDrop" Position="7442577" />
          <Marker Name="PostRaceLoopStart" Position="7761169" />
          <Marker Name="PostRaceLoopEnd" Position="8424204" />
          <Marker Name="StingerStart" Position="9536281" />
          <Marker Name="DJStart" Position="9538281" />
          <Marker Name="End" Position="9633792" />
          <Marker Name="Loop1Start" Position="-1" />
          <Marker Name="Loop1End" Position="-1" />
          <Marker Name="Loop2Start" Position="-1" />
          <Marker Name="Loop2End" Position="-1" />
          <Marker Name="Loop3Start" Position="-1" />
          <Marker Name="Loop3End" Position="-1" />
          <Marker Name="Loop4Start" Position="-1" />
          <Marker Name="Loop4End" Position="-1" />
          <Marker Name="Loop5Start" Position="-1" />
          <Marker Name="Loop5End" Position="-1" />
          <Marker Name="Section1" Position="-1" />
          <Marker Name="Section2" Position="-1" />
          <Marker Name="Section3" Position="-1" />
          <Marker Name="Section4" Position="-1" />
          <Marker Name="Section5" Position="-1" />
          <Loop Name="TrackMain" StartMarker="TrackLoopStart" EndMarker="TrackLoopEnd" />
          <Loop Name="TrackPostRace" StartMarker="PostRaceLoopStart" EndMarker="PostRaceLoopEnd" />
          <Loop Name="Loop1" StartMarker="Loop1Start" EndMarker="Loop1End" />
          <Loop Name="Loop2" StartMarker="Loop2Start" EndMarker="Loop2End" />
          <Loop Name="Loop3" StartMarker="Loop3Start" EndMarker="Loop3End" />
          <Loop Name="Loop4" StartMarker="Loop4Start" EndMarker="Loop4End" />
          <Loop Name="Loop5" StartMarker="Loop5Start" EndMarker="Loop5End" />
          <BPM Value="169.9145" Start="119916" />
          <BPM Value="169.9145" Start="6493004" />
          <BPM Value="169.9145" Start="11349624" />
        </Sample>
        <Sample SoundName="HZ5_R4_FooFighters_HoldingPoison" SampleLength="6568960" SampleRate="48000" DisplayName="In The Dark" Artist="Armin Van Buuren, David Guetta, Aldae" IsXCloudModeSafe="true">
          <Marker Name="VeryStart" Position="-1" />
          <Marker Name="TrackStart" Position="0" />
          <Marker Name="DJDrop" Position="266994" />
          <Marker Name="TrackDrop" Position="811941" />
          <Marker Name="TrackLoopStart" Position="1695226" />
          <Marker Name="TrackLoopEnd" Position="5053485" />
          <Marker Name="DJSegment" Position="3008180" />
          <Marker Name="PostDrop" Position="5723414" />
          <Marker Name="PostRaceLoopStart" Position="5871500" />
          <Marker Name="PostRaceLoopEnd" Position="6207767" />
          <Marker Name="StingerStart" Position="6461335" />
          <Marker Name="DJStart" Position="6462335" />
          <Marker Name="End" Position="6568960" />
          <Marker Name="Loop1Start" Position="-1" />
          <Marker Name="Loop1End" Position="-1" />
          <Marker Name="Loop2Start" Position="-1" />
          <Marker Name="Loop2End" Position="-1" />
          <Marker Name="Loop3Start" Position="-1" />
          <Marker Name="Loop3End" Position="-1" />
          <Marker Name="Loop4Start" Position="-1" />
          <Marker Name="Loop4End" Position="-1" />
          <Marker Name="Loop5Start" Position="-1" />
          <Marker Name="Loop5End" Position="-1" />
          <Marker Name="Section1" Position="-1" />
          <Marker Name="Section2" Position="-1" />
          <Marker Name="Section3" Position="-1" />
          <Marker Name="Section4" Position="-1" />
          <Marker Name="Section5" Position="-1" />
          <Loop Name="TrackMain" StartMarker="TrackLoopStart" EndMarker="TrackLoopEnd" />
          <Loop Name="TrackPostRace" StartMarker="PostRaceLoopStart" EndMarker="PostRaceLoopEnd" />
          <Loop Name="Loop1" StartMarker="Loop1Start" EndMarker="Loop1End" />
          <Loop Name="Loop2" StartMarker="Loop2Start" EndMarker="Loop2End" />
          <Loop Name="Loop3" StartMarker="Loop3Start" EndMarker="Loop3End" />
          <Loop Name="Loop4" StartMarker="Loop4Start" EndMarker="Loop4End" />
          <Loop Name="Loop5" StartMarker="Loop5Start" EndMarker="Loop5End" />
          <BPM Value="86.4587" Start="121277" />
          <BPM Value="86.4587" Start="3152550" />
          <BPM Value="86.4587" Start="7616184" />
        </Sample>
        <Sample SoundName="HZ5_R4_MeltedBrains_IWannaConnect" SampleLength="9653248" SampleRate="48000" DisplayName="Take You Home" Artist="Jason Ross ft Dia Frampton" IsXCloudModeSafe="true">
          <Marker Name="VeryStart" Position="-1" />
          <Marker Name="TrackStart" Position="0" />
          <Marker Name="DJDrop" Position="113568" />
          <Marker Name="TrackDrop" Position="1188675" />
          <Marker Name="TrackLoopStart" Position="2279234" />
          <Marker Name="TrackLoopEnd" Position="6109938" />
          <Marker Name="DJSegment" Position="5105095" />
          <Marker Name="PostDrop" Position="3916608" />
          <Marker Name="PostRaceLoopStart" Position="4621991" />
          <Marker Name="PostRaceLoopEnd" Position="5027197" />
          <Marker Name="StingerStart" Position="9468518" />
          <Marker Name="DJStart" Position="9469518" />
          <Marker Name="End" Position="9653248" />
          <Marker Name="Loop1Start" Position="-1" />
          <Marker Name="Loop1End" Position="-1" />
          <Marker Name="Loop2Start" Position="-1" />
          <Marker Name="Loop2End" Position="-1" />
          <Marker Name="Loop3Start" Position="-1" />
          <Marker Name="Loop3End" Position="-1" />
          <Marker Name="Loop4Start" Position="-1" />
          <Marker Name="Loop4End" Position="-1" />
          <Marker Name="Loop5Start" Position="-1" />
          <Marker Name="Loop5End" Position="-1" />
          <Marker Name="Section1" Position="-1" />
          <Marker Name="Section2" Position="-1" />
          <Marker Name="Section3" Position="-1" />
          <Marker Name="Section4" Position="-1" />
          <Marker Name="Section5" Position="-1" />
          <Loop Name="TrackMain" StartMarker="TrackLoopStart" EndMarker="TrackLoopEnd" />
          <Loop Name="TrackPostRace" StartMarker="PostRaceLoopStart" EndMarker="PostRaceLoopEnd" />
          <Loop Name="Loop1" StartMarker="Loop1Start" EndMarker="Loop1End" />
          <Loop Name="Loop2" StartMarker="Loop2Start" EndMarker="Loop2End" />
          <Loop Name="Loop3" StartMarker="Loop3Start" EndMarker="Loop3End" />
          <Loop Name="Loop4" StartMarker="Loop4Start" EndMarker="Loop4End" />
          <Loop Name="Loop5" StartMarker="Loop5Start" EndMarker="Loop5End" />
          <BPM Value="104.4278" Start="21032" />
          <BPM Value="104.4278" Start="5978064" />
        </Sample>
        <Sample SoundName="HZ5_R4_NothingButThieves_Unperson" SampleLength="6578176" SampleRate="48000" DisplayName="Loca Loca (Vion Konger Remix)" Artist="R3HAB" IsXCloudModeSafe="true">
          <Marker Name="VeryStart" Position="-1" />
          <Marker Name="TrackStart" Position="0" />
          <Marker Name="DJDrop" Position="50277" />
          <Marker Name="TrackDrop" Position="355756" />
          <Marker Name="TrackLoopStart" Position="656503" />
          <Marker Name="TrackLoopEnd" Position="3957423" />
          <Marker Name="DJSegment" Position="2638282" />
          <Marker Name="PostDrop" Position="5245887" />
          <Marker Name="PostRaceLoopStart" Position="5928742" />
          <Marker Name="PostRaceLoopEnd" Position="6235079" />
          <Marker Name="StingerStart" Position="6516020" />
          <Marker Name="DJStart" Position="6517020" />
          <Marker Name="End" Position="6578176" />
          <Marker Name="Loop1Start" Position="-1" />
          <Marker Name="Loop1End" Position="-1" />
          <Marker Name="Loop2Start" Position="-1" />
          <Marker Name="Loop2End" Position="-1" />
          <Marker Name="Loop3Start" Position="-1" />
          <Marker Name="Loop3End" Position="-1" />
          <Marker Name="Loop4Start" Position="-1" />
          <Marker Name="Loop4End" Position="-1" />
          <Marker Name="Loop5Start" Position="-1" />
          <Marker Name="Loop5End" Position="-1" />
          <Marker Name="Section1" Position="-1" />
          <Marker Name="Section2" Position="-1" />
          <Marker Name="Section3" Position="-1" />
          <Marker Name="Section4" Position="-1" />
          <Marker Name="Section5" Position="-1" />
          <Loop Name="TrackMain" StartMarker="TrackLoopStart" EndMarker="TrackLoopEnd" />
          <Loop Name="TrackPostRace" StartMarker="PostRaceLoopStart" EndMarker="PostRaceLoopEnd" />
          <Loop Name="Loop1" StartMarker="Loop1Start" EndMarker="Loop1End" />
          <Loop Name="Loop2" StartMarker="Loop2Start" EndMarker="Loop2End" />
          <Loop Name="Loop3" StartMarker="Loop3Start" EndMarker="Loop3End" />
          <Loop Name="Loop4" StartMarker="Loop4Start" EndMarker="Loop4End" />
          <Loop Name="Loop5" StartMarker="Loop5Start" EndMarker="Loop5End" />
          <BPM Value="102.9531" Start="8807" />
          <BPM Value="102.9531" Start="10974581" />
        </Sample>
        <Sample SoundName="HZ5_R4_PlagueVendor_NewComedown" SampleLength="9190002" SampleRate="48000" DisplayName="Won't Let You Go" Artist="Martin Garrix" IsXCloudModeSafe="true">
          <Marker Name="VeryStart" Position="-1" />
          <Marker Name="TrackStart" Position="0" />
          <Marker Name="DJDrop" Position="0" />
          <Marker Name="TrackDrop" Position="1322289" />
          <Marker Name="TrackLoopStart" Position="3405780" />
          <Marker Name="TrackLoopEnd" Position="7770166" />
          <Marker Name="DJSegment" Position="4814709" />
          <Marker Name="PostDrop" Position="7758621" />
          <Marker Name="PostRaceLoopStart" Position="8382264" />
          <Marker Name="PostRaceLoopEnd" Position="9055462" />
          <Marker Name="StingerStart" Position="9134146" />
          <Marker Name="DJStart" Position="9135146" />
          <Marker Name="End" Position="9190002" />
          <Marker Name="Loop1Start" Position="-1" />
          <Marker Name="Loop1End" Position="-1" />
          <Marker Name="Loop2Start" Position="-1" />
          <Marker Name="Loop2End" Position="-1" />
          <Marker Name="Loop3Start" Position="-1" />
          <Marker Name="Loop3End" Position="-1" />
          <Marker Name="Loop4Start" Position="-1" />
          <Marker Name="Loop4End" Position="-1" />
          <Marker Name="Loop5Start" Position="-1" />
          <Marker Name="Loop5End" Position="-1" />
          <Marker Name="Section1" Position="-1" />
          <Marker Name="Section2" Position="-1" />
          <Marker Name="Section3" Position="-1" />
          <Marker Name="Section4" Position="-1" />
          <Marker Name="Section5" Position="-1" />
          <Loop Name="TrackMain" StartMarker="TrackLoopStart" EndMarker="TrackLoopEnd" />
          <Loop Name="TrackPostRace" StartMarker="PostRaceLoopStart" EndMarker="PostRaceLoopEnd" />
          <Loop Name="Loop1" StartMarker="Loop1Start" EndMarker="Loop1End" />
          <Loop Name="Loop2" StartMarker="Loop2Start" EndMarker="Loop2End" />
          <Loop Name="Loop3" StartMarker="Loop3Start" EndMarker="Loop3End" />
          <Loop Name="Loop4" StartMarker="Loop4Start" EndMarker="Loop4End" />
          <Loop Name="Loop5" StartMarker="Loop5Start" EndMarker="Loop5End" />
          <BPM Value="172.2923" Start="11069" />
          <BPM Value="172.2923" Start="9706222" />
        </Sample>
        <Sample SoundName="HZ5_R4_SOFITUKKER_Freak" SampleLength="7113728" SampleRate="48000" DisplayName="Crab Rave" Artist="Noisestorm" IsXCloudModeSafe="true">
          <Marker Name="VeryStart" Position="-1" />
          <Marker Name="TrackStart" Position="0" />
          <Marker Name="DJDrop" Position="673486" />
          <Marker Name="TrackDrop" Position="1307383" />
          <Marker Name="TrackLoopStart" Position="2025293" />
          <Marker Name="TrackLoopEnd" Position="4735500" />
          <Marker Name="DJSegment" Position="3391967" />
          <Marker Name="PostDrop" Position="4735500" />
          <Marker Name="PostRaceLoopStart" Position="5768013" />
          <Marker Name="PostRaceLoopEnd" Position="5937603" />
          <Marker Name="StingerStart" Position="6882487" />
          <Marker Name="DJStart" Position="6883487" />
          <Marker Name="End" Position="7113728" />
          <Marker Name="Loop1Start" Position="-1" />
          <Marker Name="Loop1End" Position="-1" />
          <Marker Name="Loop2Start" Position="-1" />
          <Marker Name="Loop2End" Position="-1" />
          <Marker Name="Loop3Start" Position="-1" />
          <Marker Name="Loop3End" Position="-1" />
          <Marker Name="Loop4Start" Position="-1" />
          <Marker Name="Loop4End" Position="-1" />
          <Marker Name="Loop5Start" Position="-1" />
          <Marker Name="Loop5End" Position="-1" />
          <Marker Name="Section1" Position="-1" />
          <Marker Name="Section2" Position="-1" />
          <Marker Name="Section3" Position="-1" />
          <Marker Name="Section4" Position="-1" />
          <Marker Name="Section5" Position="-1" />
          <Loop Name="TrackMain" StartMarker="TrackLoopStart" EndMarker="TrackLoopEnd" />
          <Loop Name="TrackPostRace" StartMarker="PostRaceLoopStart" EndMarker="PostRaceLoopEnd" />
          <Loop Name="Loop1" StartMarker="Loop1Start" EndMarker="Loop1End" />
          <Loop Name="Loop2" StartMarker="Loop2Start" EndMarker="Loop2End" />
          <Loop Name="Loop3" StartMarker="Loop3Start" EndMarker="Loop3End" />
          <Loop Name="Loop4" StartMarker="Loop4Start" EndMarker="Loop4End" />
          <Loop Name="Loop5" StartMarker="Loop5Start" EndMarker="Loop5End" />
          <BPM Value="66.97887" Start="2543" />
          <BPM Value="66.97887" Start="5850357" />
        </Sample>
        <Sample SoundName="HZ5_R4_WolfAlice_Smile" SampleLength="10445824" SampleRate="48000" DisplayName="Stargazing" Artist="Kygo ft Justin Jesso" IsXCloudModeSafe="true">
          <Marker Name="VeryStart" Position="-1" />
          <Marker Name="TrackStart" Position="0" />
          <Marker Name="DJDrop" Position="368676" />
          <Marker Name="TrackDrop" Position="1196149" />
          <Marker Name="TrackLoopStart" Position="2105550" />
          <Marker Name="TrackLoopEnd" Position="5849661" />
          <Marker Name="DJSegment" Position="4952811" />
          <Marker Name="PostDrop" Position="8450173" />
          <Marker Name="PostRaceLoopStart" Position="8666961" />
          <Marker Name="PostRaceLoopEnd" Position="9096059" />
          <Marker Name="StingerStart" Position="10236302" />
          <Marker Name="DJStart" Position="10237302" />
          <Marker Name="End" Position="10445824" />
          <Marker Name="Loop1Start" Position="-1" />
          <Marker Name="Loop1End" Position="-1" />
          <Marker Name="Loop2Start" Position="-1" />
          <Marker Name="Loop2End" Position="-1" />
          <Marker Name="Loop3Start" Position="-1" />
          <Marker Name="Loop3End" Position="-1" />
          <Marker Name="Loop4Start" Position="-1" />
          <Marker Name="Loop4End" Position="-1" />
          <Marker Name="Loop5Start" Position="-1" />
          <Marker Name="Loop5End" Position="-1" />
          <Marker Name="Section1" Position="-1" />
          <Marker Name="Section2" Position="-1" />
          <Marker Name="Section3" Position="-1" />
          <Marker Name="Section4" Position="-1" />
          <Marker Name="Section5" Position="-1" />
          <Loop Name="TrackMain" StartMarker="TrackLoopStart" EndMarker="TrackLoopEnd" />
          <Loop Name="TrackPostRace" StartMarker="PostRaceLoopStart" EndMarker="PostRaceLoopEnd" />
          <Loop Name="Loop1" StartMarker="Loop1Start" EndMarker="Loop1End" />
          <Loop Name="Loop2" StartMarker="Loop2Start" EndMarker="Loop2End" />
          <Loop Name="Loop3" StartMarker="Loop3Start" EndMarker="Loop3End" />
          <Loop Name="Loop4" StartMarker="Loop4Start" EndMarker="Loop4End" />
          <Loop Name="Loop5" StartMarker="Loop5Start" EndMarker="Loop5End" />
          <BPM Value="52.1" Start="105136" />
          <BPM Value="52.1" Start="3642947" />
        </Sample>
...
```

- Add these 10 lines (Entry) in the FreeRoam and Event playlist (which is in the ``<RadioStation Name="Horizon Bass Arena" Number="2">`` section too)
```xml
...
    <PlayList Type="FreeRoam">
        ...
        <Entry Name="HZ5_R4_AngelicaGarcia_KarmaTheKnife" />
        <Entry Name="HZ5_R4_BiteTheBuffalo_Getaway" />
        <Entry Name="HZ5_R4_FooFighters_HoldingPoison" />
        <Entry Name="HZ5_R4_DeathValleyGirls_10DayMiracleChallenge" />
        <Entry Name="HZ5_R4_ElShirota_LaCiudad" />
        <Entry Name="HZ5_R4_MeltedBrains_IWannaConnect" />
        <Entry Name="HZ5_R4_NothingButThieves_Unperson" />
        <Entry Name="HZ5_R4_PlagueVendor_NewComedown" />
        <Entry Name="HZ5_R4_SOFITUKKER_Freak" />
        <Entry Name="HZ5_R4_WolfAlice_Smile" />
    </PlayList>
    <PlayList Type="Event">
        ...
        <Entry Name="HZ5_R4_AngelicaGarcia_KarmaTheKnife" />
        <Entry Name="HZ5_R4_BiteTheBuffalo_Getaway" />
        <Entry Name="HZ5_R4_FooFighters_HoldingPoison" />
        <Entry Name="HZ5_R4_DeathValleyGirls_10DayMiracleChallenge" />
        <Entry Name="HZ5_R4_ElShirota_LaCiudad" />
        <Entry Name="HZ5_R4_MeltedBrains_IWannaConnect" />
        <Entry Name="HZ5_R4_NothingButThieves_Unperson" />
        <Entry Name="HZ5_R4_PlagueVendor_NewComedown" />
        <Entry Name="HZ5_R4_SOFITUKKER_Freak" />
        <Entry Name="HZ5_R4_WolfAlice_Smile" />
    </PlayList>
...
```

- Delete all lines (Entry) which are not included in this XML list (in the ``<RadioStation Name="Horizon XS" Number="4">`` section too):
```xml
...
    <PlayList Type="FreeRoam">
        <Entry Name="HZ5_R4_TheStruts_WildChild_feat_TomMorello" />
        <Entry Name="HZ5_R4_PlagueVendor_LiveMore" />
        <Entry Name="HZ5_R4_Maxband_Unsaid" />
        <Entry Name="HZ5_R4_RoyalBlood_TroublesComing" />
        <Entry Name="HZ5_R4_TheKillers_Caution" />
        <Entry Name="HZ5_R4_OscarLang_AntidoteToBeingBored" />
        <Entry Name="HZ5_R4_Arkells_KFlay_YouCanGetIt" />
        <Entry Name="HZ5_R4_BringMeTheHorizon_Teardrops" />
        <Entry Name="HZ5_R4_TechnicolorFabrics_MejorQueNadie" />
        <Entry Name="HZ5_R4_DIIV_UnderTheSun" />
        <Entry Name="HZ5_R4_FooFighters_NoSonOfMine" />
        <Entry Name="HZ5_R4_TheBlahBlahBlahs_DoItBetter" />
      </PlayList>
      <PlayList Type="Event">
        <Entry Name="HZ5_R4_PlagueVendor_LiveMore" />
        <Entry Name="HZ5_R4_OscarLang_AntidoteToBeingBored" />
        <Entry Name="HZ5_R4_BringMeTheHorizon_Teardrops" />
        <Entry Name="HZ5_R4_Arkells_KFlay_YouCanGetIt" />
        <Entry Name="HZ5_R4_TheBlahBlahBlahs_DoItBetter" />
        <Entry Name="HZ5_R4_TheKillers_Caution" />
        <Entry Name="HZ5_R4_Maxband_Unsaid" />
        <Entry Name="HZ5_R4_RoyalBlood_TroublesComing" />
        <Entry Name="HZ5_R4_TheStruts_WildChild_feat_TomMorello" />
        <Entry Name="HZ5_R4_TechnicolorFabrics_MejorQueNadie" />
        <Entry Name="HZ5_R4_DIIV_UnderTheSun" />
        <Entry Name="HZ5_R4_FooFighters_NoSonOfMine" />
      </PlayList>
...
```

- You have now finished the setup, you can start your game and enjoy your 10 new tracks !
