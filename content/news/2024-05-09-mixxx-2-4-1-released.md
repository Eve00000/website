title: Mixxx 2.4.1 released
authors: Evelynne Veys
tags: 2.4, 2.4.1, release announcement
comments: yes
date: 2024-05-09 15:07:38

#### Dear Mixxx-ers

The Mixxx developers started the year with good intentions and therefore imposed some deadlines on themselves.
That is why only three months after version 2.4, version 2.4.1 has been released.
This version delivers solutions for minor bugs and issues that came with 2.4.

#### What's new / What's changed / What's corrected in 2.4.1

You can download the new release from the [Download](https://mixxx.org/download/) page, the list of changes can be found in the [ChangeLog](https://github.com/mixxxdj/mixxx/blob/2.4.1/CHANGELOG.md)

##### Controller Mappings

* Behringer DDM4000 & BCR2000: Fix exception in JS code
  [#12969](https://github.com/mixxxdj/mixxx/pull/12969)
* Denon DJ MC6000MK2: Fix mapping of filter knob/button
  [#13166](https://github.com/mixxxdj/mixxx/pull/13166)
* Denon DJ MC7000: Fix redundant argument and migrate to `hotcue_x_status`
  [#13113](https://github.com/mixxxdj/mixxx/pull/13113)
  [#13121](https://github.com/mixxxdj/mixxx/pull/13121)
* Hercules Inpulse 200: Configure shift-browser knob to scroll the library (quick)
  [#12932](https://github.com/mixxxdj/mixxx/pull/12932)
* Pioneer DDJ-FLX4: Add waveform zoom and other mapping improvements
  [#12896](https://github.com/mixxxdj/mixxx/pull/12896)
  [#12842](https://github.com/mixxxdj/mixxx/pull/12842)
* Traktor Kontrol F1: Fixes for hid-parser and related script
  [#12876](https://github.com/mixxxdj/mixxx/pull/12876)
* Traktor S2 Mk1: fix warnings
  [#13145](https://github.com/mixxxdj/mixxx/pull/13145)
* Traktor S3: Fix mapping crash on macOS
  [#12840](https://github.com/mixxxdj/mixxx/pull/12840)
* Controller I/O table: sort action column by display string
  [#13039](https://github.com/mixxxdj/mixxx/pull/13039)

##### Target Support

* Fix various minor build issues
  [#12853](https://github.com/mixxxdj/mixxx/pull/12853)
  [#12847](https://github.com/mixxxdj/mixxx/pull/12847)
  [#12822](https://github.com/mixxxdj/mixxx/pull/12822)
  [#12892](https://github.com/mixxxdj/mixxx/pull/12892)
  [#13079](https://github.com/mixxxdj/mixxx/pull/13079)
  [#12989](https://github.com/mixxxdj/mixxx/pull/12989)
* CMakeLists: Always prefer OpenGL framework on macOS
  [#13080](https://github.com/mixxxdj/mixxx/pull/13080)

##### Skins

* Deere: make sampler rows persist
  [#12928](https://github.com/mixxxdj/mixxx/pull/12928)
* Tango: Remove unneeded waveform Singleton
  [#12938](https://github.com/mixxxdj/mixxx/pull/12938)
* Prevent possible crash in customs skins using parallel waveforms
  [#13043](https://github.com/mixxxdj/mixxx/pull/13043)
  [#12580](https://github.com/mixxxdj/mixxx/issues/12580)
  [#13136](https://github.com/mixxxdj/mixxx/pull/13136)
* Slider tooltip: consider orientation for up/down shortcut tooltips + add support for WKnobComposed
  [#13088](https://github.com/mixxxdj/mixxx/pull/13088)
* Tooltips: update 'hotcue' with saved loop features
  [#12875](https://github.com/mixxxdj/mixxx/pull/12875)
* Animate long press latching of sync button
  [#12990](https://github.com/mixxxdj/mixxx/pull/12990)
* Polish fx chain controls
  [#12805](https://github.com/mixxxdj/mixxx/pull/12805)

##### Library

* Sidebar: show track count and duration of History playlists
  [#12811](https://github.com/mixxxdj/mixxx/pull/12811)
  [#13020](https://github.com/mixxxdj/mixxx/pull/13020)
  [#13019](https://github.com/mixxxdj/mixxx/issues/13019)
  [#12788](https://github.com/mixxxdj/mixxx/issues/12788)
  [#12880](https://github.com/mixxxdj/mixxx/issues/12880)
  [#12882](https://github.com/mixxxdj/mixxx/pull/12882)
* Computer feature: update removable devices on Linux
  [#12893](https://github.com/mixxxdj/mixxx/pull/12893)
  [#12891](https://github.com/mixxxdj/mixxx/issues/12891)
* Playlists: Prevent removing tracks from locked playlists
  [#12927](https://github.com/mixxxdj/mixxx/pull/12927)
* History feature: Fix removing deleted tracks after export
  [#13016](https://github.com/mixxxdj/mixxx/pull/13016)
  [#13000](https://github.com/mixxxdj/mixxx/issues/13000)
* BPM display uses decimal separator of selected locale
  [#13067](https://github.com/mixxxdj/mixxx/pull/13067)
  [#13051](https://github.com/mixxxdj/mixxx/issues/13051)
* Fix relink directory when migrate between Linux/macOS and Windows
  [#12878](https://github.com/mixxxdj/mixxx/pull/12878)
* Allow adding new directories while watched directories are missing
  [#12937](https://github.com/mixxxdj/mixxx/pull/12937)
  [#10481](https://github.com/mixxxdj/mixxx/issues/10481)
* Require a minimum movement before initiating the drag&drop of tracks
  [#13135](https://github.com/mixxxdj/mixxx/pull/13135)
  [#12902](https://github.com/mixxxdj/mixxx/issues/12902)
* iTunes/Serato/Traktor/Rhythmbox: Print error if library file could not be opened
  [#13012](https://github.com/mixxxdj/mixxx/pull/13012)
* Playlists: improve table update after deleting (purging) track files
  [#13127](https://github.com/mixxxdj/mixxx/pull/13127)
* Fix Color column width issue
  [#12852](https://github.com/mixxxdj/mixxx/pull/12852)
* Tracks: select track row when clicking the preview button (only when starting preview)
  [#12791](https://github.com/mixxxdj/mixxx/pull/12791)
* Library track menu: show Hide action also in Playlist & Crates
  [#11901](https://github.com/mixxxdj/mixxx/pull/11901)

##### Miscellaneous

* Remove unnecessary unpolish operation of the style, before polish the new style
  [#12445](https://github.com/mixxxdj/mixxx/pull/12445)
* Developer Tools: Initially sort controls by group name, ascending
  [#12884](https://github.com/mixxxdj/mixxx/pull/12884)
* Waveforms: Fix scratching crossing loop boundaries
  [#13007](https://github.com/mixxxdj/mixxx/pull/13007)
* Prohibit un-replace when deck is playing
  [#13023](https://github.com/mixxxdj/mixxx/pull/13023)
  [#12906](https://github.com/mixxxdj/mixxx/issues/12906)
* Track Properties dialog: Prevent wiping metadata when applying twice quickly
  [#12965](https://github.com/mixxxdj/mixxx/pull/12965)
  [#12963](https://github.com/mixxxdj/mixxx/issues/12963)
* AutoDJ: Fix button state after error message about playing deck 3/4
  [#12976](https://github.com/mixxxdj/mixxx/pull/12976)
  [#12975](https://github.com/mixxxdj/mixxx/issues/12975)
* Tagfetcher: Cache fetched covers
  [#12301](https://github.com/mixxxdj/mixxx/pull/12301)
  [#11084](https://github.com/mixxxdj/mixxx/issues/11084)
* Avoid beats iterator being one off and DEBUG_ASSERT in Beats::iteratorFrom
  [#13150](https://github.com/mixxxdj/mixxx/pull/13150)
  [#13149](https://github.com/mixxxdj/mixxx/issues/13149)
* Show hint if resource path in CMakeCache.txt does not exist
  [#12929](https://github.com/mixxxdj/mixxx/pull/12929)
* Always calculate the auto value for colorful console output.
  [#13153](https://github.com/mixxxdj/mixxx/pull/13153)
* Fix FLAC recording on macOS and Windows
  [#10880](https://github.com/mixxxdj/mixxx/issues/10880)
  [#13154](https://github.com/mixxxdj/mixxx/pull/13154)

#### What happened?

I would like to share some memorable moments from the [Zulip](https://mixxx.zulipchat.com/login/)-chat that are significant for the atmosphere and motivation of the Mixxx team:

##### Not giving up...

Ten days ago a Mixxx-er posted a problem that he struggled with for over a year.
He was unable to make a MIDI-connection between his Pioneer DJM-750MK2 Mixer with Mixxx and then activate the DVS (Digital Vinyl System) to work with Mixxx's Vinyl Control.
A Mixxx developer took the challenge and during 2 weeks you could see the messages flying over: log-files, screenshots, debugging-info, tooltests, capturing communication, a new pull request...
I think I've seen over 100 messages.
Trying things, fail, one step forward, two steps back ...
After two weeks the Mixxx developer managed to get it fixed.
All from a distance, not having the hardware available, putting a lot of time in it.
It was fantastic to be a witness of this magic.  
*Shout out to [Niko/Swiftb0y](https://mixxx.org/news/author/nikolaus-einhauser/) !*

##### Wow!

About three weeks ago a Mixxx developer proposed a new feature: showing the remaining beats till the next cue point in the waveform.
After some writing, testing, rewriting ... he created a feature I couldn't do without anymore.
If you make a hotcue at eg. a climax, or a loop, or an intro start in a song, you can see the remaining time (or number beats) until this point in the waveform.
Once a DJ has used this feature, they can't live without it.
This feature will be available in the next stable version 2.5  
*Shout out to [m0dB](https://github.com/m0dB) !*

#### What's going on in the Mixxx team?

* At the moment some people are trying to get Mixxx ready for stems. Stems are a new multi-channel format of audio files with which DJ's can 'remix' the song on-the-fly.
* A lot of people are improving controller-mappings to support more hardware with more features.
* Research is ongoing to make Mixxx able to share its database over a network.
* There's someone very keen on giving Mixxx the ability to support Spatial Audio.
* Translators are very busy adapting the manual and interface.
* Developers continue improving features, correcting minor bugs, and adapting code to support more machines and operating systems.
* On daily basis Mixxx-ers are given adequate support for small or big problems. Every question is taken seriously.

There is no cure for the spreading Mixxx-virus, everyone is invited to [join the Mixxx team](https://mixxx.org/get-involved/).

#### Appeal

I want to take the opportunity to make an appeal to all Mixxx-ers:
As we try to explain Mixxx's features in an optimal way and try to give the best possible support to every user, not everyone understands the English language as well as others.
Especially when the language contains technical terms it can get confusing for not native speakers.
If you understand the English manual well and you notice missing translations in your own language, please take the time to translate a/some part(s).
It needs a little effort in the beginning, but you can make a huge difference for other users.
We are available to get you started.
[Translators Wanted](https://mixxx.org/get-involved/#translators)

#### Who's writing this?

Music was my first love and it will be my last.
I like music, from Aaliyah to ZZ Top, from A Capella and Classical Aria's to Zouk, as long as it has a soul.
Since I was very young I discovered the power of music, it can strengthen or change emotions.
When I was thirteen (in the 80's) I started making my own radio show for myself, playing discs I found in my fathers (huge) collection.
A family party started my DJ-career, I felt the joy of sharing music, making people happy with it, make them want to dance.

In the late 90's I got involved with BPM Studio, a superb but dated program. Dated because it was only compatible with MP3 and WAV.
Soundquality was and is very important for me, the term audiophile describes me very well, so I don't want to make a compromise in the audio quality.
Believe me, in the 90's, early 00's harddrive space wasn't that obvious and WAV-files took a lot of space.

BPM development stopped about ten years ago and Traktor worked fine for me until a couple of years ago.
I could no longer trust and rely on Traktor for live gigs and I rediscovered Mixxx, with the versions 2.3.5/6 a big step was made.

I found a controller-mapping file (+10 years old) for my Denon HC4500 that worked fine.
My first test: Auto-DJ (autopilot in Traktor)
The software must be able to play music for days without an error = test of hardware and software.
Mixxx passed the test gloriously.
So started playing around with Mixxx, I started importing my live-library, playlists, crates and history, found some minor bugs which I discussed on the forum and in bugreports.

I got more and more interested.
I found some translation problems so I offered to make the Dutch translate of the Mixxx-application.
Meanwhile I started diving and swimming in the code to tweak some minor things, like exporting statusfiles, nowplaying, writing a new cpontroller-mappingsfile.
To give something back to the Mixxx-community I answered questions about little problems in the forum, I translated the manual and I offered to write this announcement that became a sort of testimony.

And that all in about 12 weeks since I did the Auto DJ test.
