title: Mixxx 2.4.1 released
authors: Evelynne Veys
tags: 2.4, 2.4.1, release announcement
comments: yes
status: draft

Dear Mixxx-ers,

The Mixxx-developingteam started the year with good intentions and therefore imposed itself some deadlines. That is why only two months after version 2.4, 
the next release: version 2.4.1 can be offered. This isn't just a service release fixing some minor bugs and problems, version 2.4.1 contains some nice
features. Hiding them longer for you could possibly been seen as a crime.

Before listing the details, I would like to share some memorable moments I could follow in the Zulip-chat that are significant for the atmosphere and
motivation of the Mixxx-team:

* Ten days ago a Mixxx-er posted a problem that he struggled with for over a year. He was unable to make a MIDI-connection between his Pioneer
* DJM-750MK2 Mixer with Mixxx and then activate the DVS (Digital Vinyl System) to work with Mixxx's Vinyl Control. A Mixxx-developer took the challenge and
* during 2 weeks you could see the messages flying over: log-files, screenshots, debugging-info, tooltests, capturing communication, a new pull request...
* I think I've seen over 100 messages. Trying things, fail, one step forward, two steps back ... After two weeks the Mixxx-developer managed to get it fixed.
* All on distance, not having the hardware available, putting a lot of time in it. It was fantastic to be a witness of this magic.
* Shout out to N/S!

* About three weeks ago a Mixxx-developer proposed a new feature: showing the remaining beats till the next cue point in the waveform.
* After some writing, testing, rewriting ... he created a feature I couldn't miss anymore. If you make a hotcue at eg. a climax or a loop or an intro start
* in a song you can see the remaining time (or # beats) until this point in the waveform. Once a DJ has used this feature, she/he/they can't without it.
* This feature will be available in the 2.5
* Shout out to m!

What's going on in the Mixxx-team?
* At the moment some people are trying to get Mixxx ready for stem-files, stem-files are a new multi-channel format of audio files with which DJ's can 'remix'
* the song on-the-fly.
* A lot of people are improving controller-mappings to support more hardware with more features.
* Research is ongoing to make Mixxx able to share it's database over lan.
* There's someone very keen on giving Mixxx the ability for Spatial Audio.
* Translators are very busy adapting the manual and interface.
* Developers continue improving features, correcting minor bugs, adapting code to support more machines and operating systems.
* On daily basis Mixxx-ers are given adequate support for small or big problems. Every question is taken serious.

No cure for the spreading Mixxx-virus, you 're all invited to join the Mixxx-team. 

I want to take the opportunity to make an appeal to all Mixxx-ers:
As we try to explain the Mixxx-features in an optimal way and try to give the best possible support to every user, not everyone understands the English 
language as well as others. Especially when the language contains technical terms it can get confusing for not native speakers.
If you understand the English manual well and you notice missing translations in your own language, please take the time to translate a/some part(s).
It needs a little effort in the beginning, but you can make a huge difference for other users.
We do are available to get you started.

You can download the new release from the [Download](https://mixxx.org/download/) page. 
The test release with new features will be available soon.


And now the 'what's new / what's changed / what's corrected' in 2.4.1: 

Controller Mappings
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
* Behringer DDM4000 & BCR2000: Fix exception in JS code
  [#12969](https://github.com/mixxxdj/mixxx/pull/12969)
* Denon DJ MC7000: Fix redundant argument and migrate to `hotcue_x_status`
  [#13113](https://github.com/mixxxdj/mixxx/pull/13113)
  [#13121](https://github.com/mixxxdj/mixxx/pull/13121)
* Polish fx chain controls
  [#12805](https://github.com/mixxxdj/mixxx/pull/12805)
* Controller I/O table: sort action column by display string
  [#13039](https://github.com/mixxxdj/mixxx/pull/13039)

Target Support
* Deere: make sampler rows persist
  [#12928](https://github.com/mixxxdj/mixxx/pull/12928)
* Tango: Remove unneeded waveform Singleton
  [#12938](https://github.com/mixxxdj/mixxx/pull/12938)
* Possible crash in customs skins using parallel waveforms
  [#13043](https://github.com/mixxxdj/mixxx/pull/13043)
  [#12580](https://github.com/mixxxdj/mixxx/issues/12580)
* Possible crash in customs skins using parallel waveforms
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

Library
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

Miscellaneous
* AutoDJ: Fix button state after error message about playing deck 3/4
  [#12976](https://github.com/mixxxdj/mixxx/pull/12976)
  [#12975](https://github.com/mixxxdj/mixxx/issues/12975)
* Tagfetcher: Cache fetched covers
  [#12301](https://github.com/mixxxdj/mixxx/pull/12301)
  [#11084](https://github.com/mixxxdj/mixxx/issues/11084)
* Tagfetcher: Cache fetched covers
  [#12301](https://github.com/mixxxdj/mixxx/pull/12301)
  [#11084](https://github.com/mixxxdj/mixxx/issues/11084)
* Avoid iterator being one off and DEBUG_ASSERT in Beats::iteratorFrom
  [#13150](https://github.com/mixxxdj/mixxx/pull/13150)
  [#13149](https://github.com/mixxxdj/mixxx/issues/13149)
* Show hint if resource path in CMakeCache.txt does not exist
  [#12929](https://github.com/mixxxdj/mixxx/pull/12929)
* Always calculate the auto value for colorful console output.
  [#13153](https://github.com/mixxxdj/mixxx/pull/13153)
* Fix FLAC recording on macOS and Windows
  [#10880](https://github.com/mixxxdj/mixxx/issues/10880)
  [#13154](https://github.com/mixxxdj/mixxx/pull/13154)

You can find the list also on https://github.com/mixxxdj/mixxx/blob/2.4.1/CHANGELOG.md  

