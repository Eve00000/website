title: Mixxx 2.5 Release Announcement
authors: Evelynne Veys
tags: 2.5, release announcement
comments: yes
status: draft

#### All I want for DJ-ing is ...

Home alone? Scrooged? The sound of music? Die hard?
Change plans: this year you will be having something better to do than watching old Christmas movies.
Mixxx is now your secret "Santa comin' to town", our elves had "good hearts with the burning desire to work hard",
to get you "Rockin' around the Christmas tree at the party hop" with "something mighty sweet to see".
"For the present, look high, not low": Mixxx's "presents 'neath the tree"

#### So this is the last goodbye ...

Important: OS-Support.
macOS versions earlier than 11 can have a "Last Christmas".
Windows versions earlier than version 10 build 1809 can be "Driving home for Christmas".
For Ubuntu versions earlier than 22.04 "Christmas Will Break Your Heart".
By stepping over from QT5 to QT6.5 Mixxx has to respect the minimum system requirements stated by QT for the official builds.
That's why the support has been dropped for macOS earlier than 11, Windows versions earlier then version 10 buikd 1889 and Ubuntu earlier then 22.04.

#### Let's cheer for the elves

Ho Ho Ho, our sleigh is filled with many shiny presents:

* A red box filled with brand new waveform textures and features: 'SlipMode waveform' gives you visual aid
while scratchin', the 'beats until next marker' helps you never missing the break, the GL ES support makes it
run smooth and many more...

@Video([https://youtu.be/QUuiu7BlCzI])

@Video([https://youtu.be/Xi3Ec0Jo-z8])

* With a nice yellow bow around it, the new Skin & Interface features: the menubar can be hidden,
reworked toggles (fullscreen, cue popup, vinyl control), improved tooltips, improved controls and checks (AutoDJ,
effects), new command line interface options...

@Video([https://youtu.be/tUYfLxeQh2o])

* Our engine became a V8 sleigh: undo function for BPM/beats, beatloop anchor, rate tap button...
* "Rudolph, the Red-Nosed Reindeer" will sound much better with the compressor and glitch effects and the improved backend.

@Video([https://youtu.be/W2Gjdv3R6BM])

* Your "Jingles" and "Bells" can be sorted and found easier with the new library features: Cut, Copy and Paste in tracklists,
tracks can be moved with ALT+Up/Down/PgUp/PgDn, the searchengine received new BPM filters, an 'OR'-operator, new import possibilities,
custom track colors for missing or played tracks ...

@Video([https://youtu.be/IOUv255xH20])

* "Santa Tell Me" what's new in preferences: some improved layout, the fetching of the soundcard's sample rate is fixed,
a new setting for 'first hotcue', multiple options can be selected in the MIDI input editor...
* Many "Days Of Christmas" full of improved Controller Mappings for Denon MC7000, Numark Scratch, Pioneer DDJ-FLX4, Traktor Kontrol S4 MK3 and MIDI for light.
* A Controller Backend as a "Fairytale of New York" to map your controller: sysex, deck's track menu, support for bulk devices,
drop of lodash dependency...
* The experimental QML Skin is a "Player’s Ball", an appetizer for the future GUI of Mixxx.
* QT5 will Be Home For Christmas because Mixxx is using [QT6](https://www.qt.io/product/qt6) now, a lot of work has been put
in study, preparation, testing, upgrading procedures, adapting routines, dialogs, widgets, libraries.
Upgrading to QT6 wasn't just sitting "underneath the Mistletoe" but now Mixxx is in "Winter Wonderland".
"Thank you Santa" Developers!
* "Feliz" iOs & WebAssembly: experiments are on-going to run Mixxx on iOs and in a Webbrowser.
* So many rafactorings have been made, improvements of the code by progressive insight, because of new
possibilities in c++ and QT, because of studies in acoustics, user experiences...
The list is too long to write or make a selection here, it would be failing all contributors,
you can find the complete list further in this announcement, full of "Christmas Lights"


#### So this is Christmas

"Baby, It's Cold Outside", so our present will be lots of fun exploring this new version.
You'll need quiet some time to get used to all new features, discover the real possibilities,
to get some adapted workflow with new handles.
Mixxx whishes you a "Wonderful Christmas Time".

Mic drop, "Light the Candles All Around the World"


#### ... and a happy 2.5


### Waveforms

* SlipMode waveform visual for RGB GLSL
  [#13002](https://github.com/mixxxdj/mixxx/pull/13002)
  [#13256](https://github.com/mixxxdj/mixxx/pull/13256)
* Show beats and time until next marker in the waveform
  [#12994](https://github.com/mixxxdj/mixxx/pull/12994)
  [#13311](https://github.com/mixxxdj/mixxx/pull/13311)
* Waveforms: don't elide hotcue labels
  [#13219](https://github.com/mixxxdj/mixxx/pull/13219)
  [#10722](https://github.com/mixxxdj/mixxx/issues/10722)
* Waveforms: Allshader RGB, Filtered and Stacked Waveforms using textures for waveform data
  [#13151](https://github.com/mixxxdj/mixxx/pull/13151)
  [#12641](https://github.com/mixxxdj/mixxx/issues/12641)
* Allow changing the waveform overview type without reloading the skin
  [#13273](https://github.com/mixxxdj/mixxx/pull/13273)
* Maintain GL ES support
  [#13485](https://github.com/mixxxdj/mixxx/pull/13485)
* Update overview immediately, when the normalize option or global gain changed [#13634](https://github.com/mixxxdj/mixxx/pull/13634)

### Skins / Interface

* Toggle the menubar with single Alt key press (auto hide)
  [#11526](https://github.com/mixxxdj/mixxx/pull/11526)
  [#13301](https://github.com/mixxxdj/mixxx/pull/13301)
* Fullscreen toggle rework [#11566](https://github.com/mixxxdj/mixxx/pull/11566)
* Allow to edit track title and artist directly within the decks via a delayed double-click
  [#11755](https://github.com/mixxxdj/mixxx/pull/11755)
  [#13930](https://github.com/mixxxdj/mixxx/pull/13930)
* Require a minimum movement before initiating the drag&drop of tracks [#12903](https://github.com/mixxxdj/mixxx/pull/12903)
* Add type toggle to cue popup [#13215](https://github.com/mixxxdj/mixxx/pull/13215)
* Effect Meta Knob: draws arc from default meta position
  [#12638](https://github.com/mixxxdj/mixxx/pull/12638)
  [#12634](https://github.com/mixxxdj/mixxx/issues/12634)
* Handle not supported files when dragging to waveforms and spinnies
  [#13206](https://github.com/mixxxdj/mixxx/issues/13206)
* Improve `rate_up/down` tooltips, pitch vs. speed [#12590](https://github.com/mixxxdj/mixxx/pull/12590)
* Add tooltip for expand/collapse samplers button
  [#13005](https://github.com/mixxxdj/mixxx/pull/13005)
  [#12998](https://github.com/mixxxdj/mixxx/issues/12998)
* LateNight: Merge vinyl control toggle and status light
  [#12947](https://github.com/mixxxdj/mixxx/pull/12947)
  [#10192](https://github.com/mixxxdj/mixxx/issues/10192)
* Track label widgets: set `show_track_menu` only for main decks [#12978](https://github.com/mixxxdj/mixxx/pull/12978)
* MacOS: App proxy icon of the playing track to the window title [#12116](https://github.com/mixxxdj/mixxx/pull/12116)
* PreviewDeckN,LoadSelectedTrackAndPlay toggles play/pause if the track is already loaded
  [#12920](https://github.com/mixxxdj/mixxx/pull/12920)
  [#9819](https://github.com/mixxxdj/mixxx/issues/9819)
* AutoDJ: Force-show decks 3/4 if we are going to use them [#13455](https://github.com/mixxxdj/mixxx/pull/13455)
* Show wait cursor when re/loading a skin (not during startup) [#13747](https://github.com/mixxxdj/mixxx/pull/13747)
* Allow to set LaunchImage style per color scheme [#13731](https://github.com/mixxxdj/mixxx/pull/13731)
* LateNight, Deere, Tango: Deactivate beatgrid edit controls if BPM is locked
  [#13320](https://github.com/mixxxdj/mixxx/pull/13320)
  [#13323](https://github.com/mixxxdj/mixxx/pull/13323)
  [#13325](https://github.com/mixxxdj/mixxx/pull/13325)
* LateNight: Add/tweak CueDelete icons
  [#13495](https://github.com/mixxxdj/mixxx/pull/13495)
  [#13492](https://github.com/mixxxdj/mixxx/issues/13492)
* LateNight: Use Classic launch image style also for 64 samplers version [#13796](https://github.com/mixxxdj/mixxx/pull/13796)
* Command line interface: Determine whether to color output based on `TERM` variable
  [#13486](https://github.com/mixxxdj/mixxx/pull/13486)
* Command line interface: Add option `--start-autodj` to start Auto DJ immediately after Mixxx start.
  [#13017](https://github.com/mixxxdj/mixxx/pull/13017)
  [#10189](https://github.com/mixxxdj/mixxx/issues/10189)
* Logging: Include timestamps in messages by default [#11861](https://github.com/mixxxdj/mixxx/pull/11861)

### Engine

* Beats: allow undoing the last BPM/beats change [#12954](https://github.com/mixxxdj/mixxx/pull/12954)
  [#12774](https://github.com/mixxxdj/mixxx/issues/12774)
  [#10138](https://github.com/mixxxdj/mixxx/issues/10138)
  [#13339](https://github.com/mixxxdj/mixxx/pull/13339)
* Add beatloop anchor to set and adjust loop from either start or end
  [#12745](https://github.com/mixxxdj/mixxx/pull/12745)
  [#13241](https://github.com/mixxxdj/mixxx/pull/13241)
* Add Rate Tap button [#12104](https://github.com/mixxxdj/mixxx/pull/12104)
* Store/restore regular loop when toggling rolling loops
  [#12475](https://github.com/mixxxdj/mixxx/pull/12475)
  [#8947](https://github.com/mixxxdj/mixxx/issues/8947)
* Add `beats_translate_move` ControlEncoder [#12376](https://github.com/mixxxdj/mixxx/pull/12376)
* Looping/Beatjump: use seconds if track has no beats
  [#12961](https://github.com/mixxxdj/mixxx/pull/12961)
  [#11124](https://github.com/mixxxdj/mixxx/issues/11124)
* Add Track colour palette cycling controls `track_color_next` and `track_color_prev` to library, decks and samplers
  [#13066](https://github.com/mixxxdj/mixxx/pull/13066)
  [#12905](https://github.com/mixxxdj/mixxx/issues/12905)
* Add Tempo locking controls
  [#13041](https://github.com/mixxxdj/mixxx/pull/13041)
  [#13041](https://github.com/mixxxdj/mixxx/pull/13041)
  [#13038](https://github.com/mixxxdj/mixxx/issues/13038)
  [#13199](https://github.com/mixxxdj/mixxx/pull/13199)

### Effects

* Add Compressor effect [#12523](https://github.com/mixxxdj/mixxx/pull/12523)
* add Glitch effect [#11329](https://github.com/mixxxdj/mixxx/pull/11329)
* Add backend for Audio Unit (AU) plugins on macOS
  [#12112](https://github.com/mixxxdj/mixxx/pull/12112)
  [#13938](https://github.com/mixxxdj/mixxx/pull/13938)
* Effect Meta knob: Draw arc from default meta position
  [#12638](https://github.com/mixxxdj/mixxx/pull/12638)
  [#12634](https://github.com/mixxxdj/mixxx/issues/12634)
* Show newly added effects, read/write HiddenEffects
  [#13326](https://github.com/mixxxdj/mixxx/pull/13326)
  [#11343](https://github.com/mixxxdj/mixxx/issues/11343)

### Library

* Shortkeys Cut, Copy, Paste for track list management
  [#12020](https://github.com/mixxxdj/mixxx/pull/12020)
  [#13361](https://github.com/mixxxdj/mixxx/issues/13361)
  [#13364](https://github.com/mixxxdj/mixxx/pull/13364)
* Track menu: Rephrase "Reset" to "Clear" [#12955](https://github.com/mixxxdj/mixxx/pull/12955)
* Playlists: move tracks with Alt + Up/Down/PageUp/PageDown/Home/End
  [#13092](https://github.com/mixxxdj/mixxx/pull/13092)
  [#10826](https://github.com/mixxxdj/mixxx/issues/10826)
  [#13098](https://github.com/mixxxdj/mixxx/pull/13098)
* Search: Add special BPM filters
  [#12072](https://github.com/mixxxdj/mixxx/pull/12072)
  [#8191](https://github.com/mixxxdj/mixxx/issues/8191)
* Search: Add "OR" search operator
  [#12061](https://github.com/mixxxdj/mixxx/pull/12061)
  [#8881](https://github.com/mixxxdj/mixxx/issues/8881)
* Search: Add 'type' filter
  [#13338](https://github.com/mixxxdj/mixxx/issues/13338)
* Search: Add 'id' filter [#13694](https://github.com/mixxxdj/mixxx/pull/13694)
* Search related Tracks menu: Allow to use multiple filters at once
  [#12213](https://github.com/mixxxdj/mixxx/pull/12213)
  [#12211](https://github.com/mixxxdj/mixxx/issues/12211)
* Add multi-track property editor / batch tag editor
  [#12548](https://github.com/mixxxdj/mixxx/pull/12548)
  [#9023](https://github.com/mixxxdj/mixxx/issues/9023)
  [#13299](https://github.com/mixxxdj/mixxx/pull/13299)
  [#13609](https://github.com/mixxxdj/mixxx/pull/13609)
  [#13597](https://github.com/mixxxdj/mixxx/issues/13597)
* Computer feature: add sidebar action "Refresh directory tree" [#12908](https://github.com/mixxxdj/mixxx/pull/12908)
* Library: Add feedback to directory operations (add, remove, relink)
  [#12436](https://github.com/mixxxdj/mixxx/pull/12436)
  [#10481](https://github.com/mixxxdj/mixxx/issues/10481)
* Library: Add support for scaling BPM by different ratios
  [#12934](https://github.com/mixxxdj/mixxx/pull/12934)
  [#9133](https://github.com/mixxxdj/mixxx/issues/9133)
* Library: Add ability to import external playlists as crates [#11852](https://github.com/mixxxdj/mixxx/pull/11852)
* Library: Add 'Shuffle playlist' sidebar action
  [#12498](https://github.com/mixxxdj/mixxx/pull/12498)
  [#6988](https://github.com/mixxxdj/mixxx/issues/6988)
* Playlists: Update of playlist labels after adding tracks [#12866](https://github.com/mixxxdj/mixxx/pull/12866) [#12761](https://github.com/mixxxdj/mixxx/issues/12761)
* Library: Custom color for missing tracks [#12895](https://github.com/mixxxdj/mixxx/pull/12895)
* Tracks: Custom text color for played tracks (qss)
  [#12744](https://github.com/mixxxdj/mixxx/pull/12744)
  [#5911](https://github.com/mixxxdj/mixxx/issues/5911)
  [#12912](https://github.com/mixxxdj/mixxx/pull/12912)
  [#13538](https://github.com/mixxxdj/mixxx/pull/13538)
* History: Show track count and duration in sidebar [#12811](https://github.com/mixxxdj/mixxx/pull/12811) [#12788](https://github.com/mixxxdj/mixxx/issues/12788)
* Fixes around cratetablemodel, remove tracks + don't allow pasting tracks into locked playlists/crates or History [#12926](https://github.com/mixxxdj/mixxx/pull/12926)
* Track menu, Remove from disk: stop and eject all affected decks [#13214](https://github.com/mixxxdj/mixxx/pull/13214)
* Track menu: add star rating
  [#12700](https://github.com/mixxxdj/mixxx/pull/12700)
  [#10652](https://github.com/mixxxdj/mixxx/issues/10652)
* Track menu: Show Properties in Missing and Hidden view [#13426](https://github.com/mixxxdj/mixxx/pull/13426)
* Optimize Library scrolling in BPMDelegate::paintItem [#13358](https://github.com/mixxxdj/mixxx/pull/13358)
* Fix font reset in multiline comment editor [#13448](https://github.com/mixxxdj/mixxx/pull/13448)
* Keep the metadata key text unchanged, use it as the origin of information
  [#11096](https://github.com/mixxxdj/mixxx/pull/11096)
  [#11095](https://github.com/mixxxdj/mixxx/issues/11095)
  [#13650](https://github.com/mixxxdj/mixxx/pull/13650)
* Center date values, right-align Track # [#13674](https://github.com/mixxxdj/mixxx/pull/13674)
* Add a debug message, which appears when event loop processing in Mixxx application takes very long
  [#12094](https://github.com/mixxxdj/mixxx/pull/12094)
  [#13900](https://github.com/mixxxdj/mixxx/pull/13900)
  [#13889](https://github.com/mixxxdj/mixxx/pull/13889)
  [#13903](https://github.com/mixxxdj/mixxx/pull/13903)
* Analysis: Fix stop button when analyzing crate/playlist [#13902](https://github.com/mixxxdj/mixxx/pull/13902)

### Preferences

* Add missing spacer in interface preferences [#13094](https://github.com/mixxxdj/mixxx/pull/13094)
* Fix fetching of soundcard sample rate
  [#11951](https://github.com/mixxxdj/mixxx/pull/11951)
  [11949](https://github.com/mixxxdj/mixxx/issues/11949)
* Add load point option 'First hotcue'
  [#12869](https://github.com/mixxxdj/mixxx/pull/12869)
  [#12740](https://github.com/mixxxdj/mixxx/issues/12740)
* MIDI Input editor: allow selecting multiple Options [#12348](https://github.com/mixxxdj/mixxx/pull/12348)
* Apply changes only after pressing Apply in color preferences [#13302](https://github.com/mixxxdj/mixxx/pull/13302)

### Controller Mappings

* Denon MC7000: Add optional jog wheel acceleration to the controller mapping [#4684](https://github.com/mixxxdj/mixxx/pull/4684)
* Denon MC7000: Unify parameter button logic and add customizable modes [#13589](https://github.com/mixxxdj/mixxx/pull/13589)
* MIDI for light: Implement new Active deck heuristic [#13513](https://github.com/mixxxdj/mixxx/pull/13513)
* Numark Scratch: Add controller settings  [#13404](https://github.com/mixxxdj/mixxx/pull/13404)
* Pioneer DDJ-FLX4: Mapping improvements [#12842](https://github.com/mixxxdj/mixxx/pull/12842)
* Traktor Kontrol S4 MK3: Add setting definition for  [#12995](https://github.com/mixxxdj/mixxx/pull/12995)
* Traktor Kontrol S4 MK3: Software mixer support and default pad layout customisation [#13059](https://github.com/mixxxdj/mixxx/pull/13059)
* Traktor Kontrol S4 Mk3: Rework jogwheel speed compute and motorized platter [#13393](https://github.com/mixxxdj/mixxx/pull/13393)

### Controller Backend

* Send sysex to all handlers [#12827](https://github.com/mixxxdj/mixxx/pull/12827)
* Add control for showing a deck's track menu [#10825](https://github.com/mixxxdj/mixxx/pull/10825)
* Removed old examples HID keyboard and HID trackpad [#12977](https://github.com/mixxxdj/mixxx/pull/12977)
* Reduce log noise with HID device
  [#13010](https://github.com/mixxxdj/mixxx/pull/13010)
  [#13125](https://github.com/mixxxdj/mixxx/pull/13125)
* Allow controller mapping to discard polling [#12558](https://github.com/mixxxdj/mixxx/pull/12558)
* Add support for mapping user settings
  [#11300](https://github.com/mixxxdj/mixxx/pull/11300)
  [#13046](https://github.com/mixxxdj/mixxx/pull/13046)
  [#13057](https://github.com/mixxxdj/mixxx/pull/13057)
  [#13045](https://github.com/mixxxdj/mixxx/pull/13045)
  [#13656](https://github.com/mixxxdj/mixxx/pull/13656)
  [#13738](https://github.com/mixxxdj/mixxx/pull/13738)
* Registering MIDI Input Handlers From Javascript
  [#12781](https://github.com/mixxxdj/mixxx/pull/12781)
  [#13089](https://github.com/mixxxdj/mixxx/pull/13089)
* Controller IO table: Fix display text for Action/control delegate [#13188](https://github.com/mixxxdj/mixxx/pull/13188)
* Drop lodash dependency in ComponentJS [#12779](https://github.com/mixxxdj/mixxx/pull/12779)
* Support for bulk devices on Windows and Mac [#13008](https://github.com/mixxxdj/mixxx/pull/13008)
* Registering MIDI Input Handlers From Javascript
  [#12781](https://github.com/mixxxdj/mixxx/pull/12781)
  [#13089](https://github.com/mixxxdj/mixxx/pull/13089)
* Drop lodash dependency in ComponentJS
  [#12779](https://github.com/mixxxdj/mixxx/pull/12779)

### Experimental QML Skin

* Add Experimental QML Skin that can be tested via the --qml command line option
  [#13152](https://github.com/mixxxdj/mixxx/pull/13152)
* Fix type error in `Slider.qml` [#11423](https://github.com/mixxxdj/mixxx/pull/11423)
* Allow switching between legacy and new QML UI with command arg [#12139](https://github.com/mixxxdj/mixxx/pull/12139)
* Add PlayerProxy missing current track when created after loading [#12559](https://github.com/mixxxdj/mixxx/pull/12559)
* Fix: Add `qt6-qpa-plugins` to dependencies [#12549](https://github.com/mixxxdj/mixxx/pull/12549)
* Fix: Improve knobs by applying selective 4xMSAA on the Arc shape [#12541](https://github.com/mixxxdj/mixxx/pull/12541)
* Add QML interceptor to auto reload on file change
  [#12795](https://github.com/mixxxdj/mixxx/pull/12795)
  [#12844](https://github.com/mixxxdj/mixxx/pull/12844)
* Add multi-sampling settings for QML [#12546](https://github.com/mixxxdj/mixxx/pull/12546)
  [#12794](https://github.com/mixxxdj/mixxx/pull/12794)
  [#12536](https://github.com/mixxxdj/mixxx/issues/12536)
  [#13058](https://github.com/mixxxdj/mixxx/pull/13058)
* Install qml module on Windows [#12604](https://github.com/mixxxdj/mixxx/pull/12604)
* Add scrolling waveforms
  [#3967](https://github.com/mixxxdj/mixxx/pull/3967)
  [#13009](https://github.com/mixxxdj/mixxx/pull/13009)
* Fix: handle case where Waveform data is missing [#13009](https://github.com/mixxxdj/mixxx/pull/13009)
* Fix: allow missing COs on QML component [#13011](https://github.com/mixxxdj/mixxx/pull/13011)
* Initialize CmdlineArgs::m_qml [#13152](https://github.com/mixxxdj/mixxx/pull/13152)
* Fix: Remove target compile defs for non-existing QML CMake target [#13506](https://github.com/mixxxdj/mixxx/pull/13506)

### Update to Qt6

* Qt6 prepare [#11863](https://github.com/mixxxdj/mixxx/pull/11863)
* Qt6 switch [#11892](https://github.com/mixxxdj/mixxx/pull/11892)
* CMakeLists: Default `QT6` to `ON` [#11934](https://github.com/mixxxdj/mixxx/pull/11934)
* Build with Qt6 and optionally with QML [#11608](https://github.com/mixxxdj/mixxx/pull/11608)
* Use constInsert() template [#11847](https://github.com/mixxxdj/mixxx/pull/11847)
* DlgAbout: Add Qt version to the dialog [#11862](https://github.com/mixxxdj/mixxx/pull/11862)
* CMakeLists: Fix `QT_TRANSLATION_FILE` path for Qt6 [#11880](https://github.com/mixxxdj/mixxx/pull/11880)
* LibraryControl: Enable control inputs for Qt6 [#11877](https://github.com/mixxxdj/mixxx/pull/11877)
* Fix wrong Windows buildenv name and missing Qt6 switch for non CI builds [#11895](https://github.com/mixxxdj/mixxx/pull/11895)
* WWidget: Disable touch events on macOS (fixing trackpad issues on Qt 6) [#11870](https://github.com/mixxxdj/mixxx/pull/11870)
* Install libjpeg-turbo::jpeg to fix cover display with Qt6 [#11922](https://github.com/mixxxdj/mixxx/pull/11922)
* Skins: Remove `border: 0px` from sidebar item styling
  [#11970](https://github.com/mixxxdj/mixxx/pull/11970)
  [#11957](https://github.com/mixxxdj/mixxx/issues/11957)
* Skins: Fix checkbox styling on Qt 6 [#12050](https://github.com/mixxxdj/mixxx/pull/12050)
* Skins: Fix Tango waveform splitter [#12939](https://github.com/mixxxdj/mixxx/pull/12939)
* Skin: Fix Tango rate range label position [#13242](https://github.com/mixxxdj/mixxx/pull/13242)
* Introduce wrapper for non const iterators for erase and insert
  [#12201](https://github.com/mixxxdj/mixxx/pull/12201)
  [#13856](https://github.com/mixxxdj/mixxx/pull/13856)
* Fix Qt6/QML build [#12255](https://github.com/mixxxdj/mixxx/pull/12255)
* Fix track color background with Qt6 [#12380](https://github.com/mixxxdj/mixxx/pull/12380)
* multi-line delegate: fix bg color, Qt6 on Linux
  [#12478](https://github.com/mixxxdj/mixxx/pull/12478)
* Revert "BaseTrackPlayer: Remove references to WaveformWidgetRenderer when using Qt6" [#12342](https://github.com/mixxxdj/mixxx/pull/12342)
* Fix: Replace deprecated `qAsConst` with `std::as_const` [#13028](https://github.com/mixxxdj/mixxx/pull/13028)
* Fix Drag'n'drop: avoid unintended drag on hover (WTrackProperty, WCoverArt etc.)
  [#13035](https://github.com/mixxxdj/mixxx/pull/13035)
  [#13033](https://github.com/mixxxdj/mixxx/issues/13033)
* Fix ambiguous overload error due to native qDebug impl for std::optional
  [#12981](https://github.com/mixxxdj/mixxx/issues/12981)
* Workaround for Qt6 'selected click' bug [#12488](https://github.com/mixxxdj/mixxx/pull/12488)
* Fix menu icon position [#12216](https://github.com/mixxxdj/mixxx/pull/12216)
* Fix/Skins: hide reserved space for invisible table header sort indicators [#13535](https://github.com/mixxxdj/mixxx/pull/13535)
* Qt 6.8 deprecated declaration fixes [#13845](https://github.com/mixxxdj/mixxx/pull/13845)
* Add missing qt6-declarative-private-dev and qt6-base-private-dev package [#13904](https://github.com/mixxxdj/mixxx/pull/13904)

### Experimental iOs support

* CMakeLists: Support building for iOS [#12672](https://github.com/mixxxdj/mixxx/pull/12672)
* DlgPrefInterface: Disable tooltips on iOS by default [#12689](https://github.com/mixxxdj/mixxx/pull/12689)
* SoundManager: Set up `AVAudioSession` on iOS [#12714](https://github.com/mixxxdj/mixxx/pull/12714)
* SoundManager: Use correct PortAudio backend on iOS [#12716](https://github.com/mixxxdj/mixxx/pull/12716)
* DesktopHelper: Add openUrl abstraction to support iOS [#12698](https://github.com/mixxxdj/mixxx/pull/12698)
* iOS packaging: Add Info.plist, launch screen and app icon [#12676](https://github.com/mixxxdj/mixxx/pull/12676)
* CmdlineArgs: Move config directory to a user-accessible location on iOS
  [#12688](https://github.com/mixxxdj/mixxx/pull/12688)
* CMakeLists: Work around Qt shader bug with Xcode
  [#13379](https://github.com/mixxxdj/mixxx/pull/13379)
  [#13378](https://github.com/mixxxdj/mixxx/issues/13378)
* AudioUnitManager: Disable unavailable in-process instantiation on iOS
  [#13383](https://github.com/mixxxdj/mixxx/pull/13383)

### Experimental WebAssembly support

* CMakeLists: Add support for targeting Emscripten/WebAssembly [#12918](https://github.com/mixxxdj/mixxx/pull/12918)
* CMakeLists: Emit better errors for exotic target platforms [#12910](https://github.com/mixxxdj/mixxx/pull/12910)
* Build: Add `PORTMIDI` flag for compiling with(out) PortMidi [#12913](https://github.com/mixxxdj/mixxx/pull/12913)
* DesktopHelper: Compile out process-spawning on WASM too [#12916](https://github.com/mixxxdj/mixxx/pull/12916)
* MixxxApplication: Use `QWasmIntegrationPlugin` when targeting WebAssembly [#12915](https://github.com/mixxxdj/mixxx/pull/12915)
* CMakeLists: Enable asyncify when targeting WASM [#12921](https://github.com/mixxxdj/mixxx/pull/12921)
* Resources: Bundle resources for preloading when targeting Emscripten/WASM [#12922](https://github.com/mixxxdj/mixxx/pull/12922)
* CMakeLists: Add `WASM_ASSERTIONS` option [#12931](https://github.com/mixxxdj/mixxx/pull/12931)
* VersionStore: Recognize Emscripten/WebAssembly [#12940](https://github.com/mixxxdj/mixxx/pull/12940)
* OpenGLWindow: Fix sizing on Wasm by setting `Qt::FramelessWindowHint` [#12945](https://github.com/mixxxdj/mixxx/pull/12945)
* CMakeLists: Require WebGL 2.0 when building for Wasm [#12952](https://github.com/mixxxdj/mixxx/pull/12952)
* ScreenSaverHelper: Add no-op implementation for WASM [#12930](https://github.com/mixxxdj/mixxx/pull/12930)
* SSE: Check `!defined(__EMSCRIPTEN__)` where intrinsics are unavailable on WASM [#12917](https://github.com/mixxxdj/mixxx/pull/12917)

### Target support

* Lenient taglib 2.0 guard [#12793](https://github.com/mixxxdj/mixxx/pull/12793)
* Tools: Add `rpm_buildenv.sh` for building on Fedora [#13069](https://github.com/mixxxdj/mixxx/pull/13069)
* README: Recommend running buildenvs over sourcing them on Linux [#13071](https://github.com/mixxxdj/mixxx/pull/13071)
* FindSndFile: Link mpg123 in static builds [#13087](https://github.com/mixxxdj/mixxx/pull/13087)
* macOS packaging: Enable app sandbox in ad-hoc-packaged (i.e. non-notarized) bundles too [#12101](https://github.com/mixxxdj/mixxx/pull/12101)
* Drop support for macOS versions earlier than 11
* Drop support for Windows versions earlier than Windows 10 build 1809
* Drop support for Ubuntu versions earlier than 22.04
* Require a C++20 compiler
* Support GCC 14.1.1
  [#13504](https://github.com/mixxxdj/mixxx/pull/13504)
  [#13467](https://github.com/mixxxdj/mixxx/issues/13467)

### Misc Refactorings

* Add missing `<Qt>` include in `defs.h` [#11348](https://github.com/mixxxdj/mixxx/pull/11348)
* Engine: Minor refactor to prefer simplified ranged-for-loop [#11234](https://github.com/mixxxdj/mixxx/pull/11234)
* Delete unused EngineFilter [#11559](https://github.com/mixxxdj/mixxx/pull/11559)
* AnalyzerWaveform: Fix commented out code [#11561](https://github.com/mixxxdj/mixxx/pull/11561)
* Remove usage of ControlObject::getControl [#11643](https://github.com/mixxxdj/mixxx/pull/11643)
* Fix unnecessary transfer of the ownership before release which returns the pointer itself [#11726](https://github.com/mixxxdj/mixxx/pull/11726)
* Add `ConfigObject::get-/setValue<EnumType>` [#11883](https://github.com/mixxxdj/mixxx/pull/11883)
* Github CI: Enable `WARNINGS_FATAL` on macOS, too [#11905](https://github.com/mixxxdj/mixxx/pull/11905)
* Refactor timers [#11807](https://github.com/mixxxdj/mixxx/pull/11807) [#11850](https://github.com/mixxxdj/mixxx/pull/11850)
* Use `mixxx::audio::ChannelCount` type instead of `int`/`unsigned char`/etc. [#11941](https://github.com/mixxxdj/mixxx/pull/11941)
* Refactor util/timer: cleanup includes [#11937](https://github.com/mixxxdj/mixxx/pull/11937)
* Use `SampleRate` type consistently [#11904](https://github.com/mixxxdj/mixxx/pull/11904)
* CMakeLists: Match arbitrary `arm64-osx` triplets [#11933](https://github.com/mixxxdj/mixxx/pull/11933)
* Reduce sample buffer memory usage [#11988](https://github.com/mixxxdj/mixxx/pull/11988)
* Fix clazy issues on `main` [#12028](https://github.com/mixxxdj/mixxx/pull/12028)
* Tidy and modernize SampleBuffer [#11987](https://github.com/mixxxdj/mixxx/pull/11987)
* Refactor parented_ptr: make trivially destructible in release mode, delete move operations [#11981](https://github.com/mixxxdj/mixxx/pull/11981)
* Labeler: Add more labels to the auto-labeler [#12106](https://github.com/mixxxdj/mixxx/pull/12106)
* FindPortMidi: Link ALSA in static builds on Linux [#12292](https://github.com/mixxxdj/mixxx/pull/12292) [#12291](https://github.com/mixxxdj/mixxx/pull/12291)
* privat generated ui headers [#12060](https://github.com/mixxxdj/mixxx/pull/12060) [#11407](https://github.com/mixxxdj/mixxx/pull/11407)
* Github CI: workaround runner-image issue [#12233](https://github.com/mixxxdj/mixxx/pull/12233)
* FindLibudev: Link hidapi and libusb with libudev in static builds on Linux [#12294](https://github.com/mixxxdj/mixxx/pull/12294)
* FindVorbis: Link ogg in static builds [#12297](https://github.com/mixxxdj/mixxx/pull/12297)
* MixxxApplication: Support linking Qt statically on Linux [#12284](https://github.com/mixxxdj/mixxx/pull/12284)
* FindSleef: Use OpenMP in static builds [#12295](https://github.com/mixxxdj/mixxx/pull/12295)
* Happy New Year 2024! [#12486](https://github.com/mixxxdj/mixxx/pull/12486)
* fix/History: remove obsolete placeholder playlists [#12494](https://github.com/mixxxdj/mixxx/pull/12494)
* Add missing Taglib dependency [#12830](https://github.com/mixxxdj/mixxx/pull/12830)
* fix: typo ;) [#12726](https://github.com/mixxxdj/mixxx/pull/12726)
* refactor: Avoid temporary qlist allocation on midi sysex receive [#12843](https://github.com/mixxxdj/mixxx/pull/12843)
* Labeler: Add `qml` to labeler config [#12911](https://github.com/mixxxdj/mixxx/pull/12911)
* WTrackMenu: Add missing wcoverartlabel.h include [#12924](https://github.com/mixxxdj/mixxx/pull/12924)
* Fix clazy complaints and naming [#12935](https://github.com/mixxxdj/mixxx/pull/12935)
* src/library: Sort files into sub-directories [#12956](https://github.com/mixxxdj/mixxx/pull/12956)
* CMakeLists: Fix deduplication trap with `--preload-file` [#12944](https://github.com/mixxxdj/mixxx/pull/12944)
* GitHub CI: Add runner that allows cleaning up the download server [#12957](https://github.com/mixxxdj/mixxx/pull/12957)
* GitHub CI: Skip the manifest update job on forks [#13278](https://github.com/mixxxdj/mixxx/pull/13278)
* Refactor FFmpeg soundsource to allow other soundsource to inherit it [#13042](https://github.com/mixxxdj/mixxx/pull/13042)
* Code Style: Add branches around single line blocks. [#13097](https://github.com/mixxxdj/mixxx/pull/13097)
* Add missing member in copy ctor [#13229](https://github.com/mixxxdj/mixxx/pull/13229)
* Refactor/preferences enums [#12798](https://github.com/mixxxdj/mixxx/pull/12798)
* localDateTimeFromUtc: Make argument a const reference and initialize QDateTime at construction [#13359](https://github.com/mixxxdj/mixxx/pull/13359)
* use enum class for waveform overview type [#13370](https://github.com/mixxxdj/mixxx/pull/13370)
* LegacySkinParser: Short-circuit if template fails to open [#13488](https://github.com/mixxxdj/mixxx/pull/13488)
* Update waveforms_container.xml [#13501](https://github.com/mixxxdj/mixxx/pull/13501)
* Disable WSwitch for generated source [#13514](https://github.com/mixxxdj/mixxx/pull/13514)
* Disable warning in lib/apple code [#13522](https://github.com/mixxxdj/mixxx/pull/13522)
* (fix) pre-commit/qsscheck: add c++ ObjectNames set via variable in [#13538](https://github.com/mixxxdj/mixxx/pull/13538) [#13549](https://github.com/mixxxdj/mixxx/pull/13549)
* chore: fix codespell complaints [#13567](https://github.com/mixxxdj/mixxx/pull/13567)
* chore: update pre-commit hook [#13530](https://github.com/mixxxdj/mixxx/pull/13530)
* chore: fix shellcheck SC2319 warning [#13569](https://github.com/mixxxdj/mixxx/pull/13569)
* Improve Taglib/SoundSource logging [#13541](https://github.com/mixxxdj/mixxx/pull/13541)
* (fix) WTrackTableView: assert track model, p prefix [#13623](https://github.com/mixxxdj/mixxx/pull/13623)
* Library control: make use of WLibrary::getCurrentTrackTableView() [#13335](https://github.com/mixxxdj/mixxx/pull/13335)
* fix: prevent crash when no app windows have the focus [#13657](https://github.com/mixxxdj/mixxx/pull/13657)
* Fix Clazy v1.12 errors in 2.5 [#13769](https://github.com/mixxxdj/mixxx/pull/13769)
* Replace module wide Qt includes to make 2.5 compliant with Clazy 1.12 [#13788](https://github.com/mixxxdj/mixxx/pull/13788)
* add missing header, fixes compilation of 2.5 on macOS [#13825](https://github.com/mixxxdj/mixxx/pull/13825)
* Fix pre-commit on F41 and update remaining dependencies [#13843](https://github.com/mixxxdj/mixxx/pull/13843)
* (fix) skin reload: store new color scheme [#13847](https://github.com/mixxxdj/mixxx/pull/13847)
* fix: eslint v9 pre-commit hook [#13886](https://github.com/mixxxdj/mixxx/pull/13886)
* clang-format: Indent Objective-C blocks with 4 spaces [#13890](https://github.com/mixxxdj/mixxx/pull/13890)
* Fix undefined behaviour of infinity() [#13884](https://github.com/mixxxdj/mixxx/pull/13884)
* Cleanup ESLint config [#13913](https://github.com/mixxxdj/mixxx/pull/13913)
* fix tsan issues
  [#13876](https://github.com/mixxxdj/mixxx/pull/13876)
  [#13869](https://github.com/mixxxdj/mixxx/issues/13869)
  [#13873](https://github.com/mixxxdj/mixxx/pull/13873)
  [#13875](https://github.com/mixxxdj/mixxx/pull/13875)
  [#13898](https://github.com/mixxxdj/mixxx/pull/13898)
  [#13899](https://github.com/mixxxdj/mixxx/pull/[#13899](https://github.com/mixxxdj/mixxx/pull/13899))
* Update to latest vcpkg dependencies
  [#11649](https://github.com/mixxxdj/mixxx/pull/11649)
  [#12512](https://github.com/mixxxdj/mixxx/pull/12512)
  [#12067](https://github.com/mixxxdj/mixxx/pull/12067)
  [#12898](https://github.com/mixxxdj/mixxx/pull/12898)
  [#13155](https://github.com/mixxxdj/mixxx/pull/13155)
  [#13830](https://github.com/mixxxdj/mixxx/pull/13830)
* GitHub actions updates
  [#11544](https://github.com/mixxxdj/mixxx/pull/11544)
  [#11508](https://github.com/mixxxdj/mixxx/pull/11508)
  [#11487](https://github.com/mixxxdj/mixxx/pull/11487)
  [#11438](https://github.com/mixxxdj/mixxx/pull/11438)
  [#11410](https://github.com/mixxxdj/mixxx/pull/11410)
  [#11560](https://github.com/mixxxdj/mixxx/pull/11560)
  [#11578](https://github.com/mixxxdj/mixxx/pull/11578)
  [#11610](https://github.com/mixxxdj/mixxx/pull/11610)
  [#11631](https://github.com/mixxxdj/mixxx/pull/11631)
  [#11710](https://github.com/mixxxdj/mixxx/pull/11710)
  [#11736](https://github.com/mixxxdj/mixxx/pull/11736)
  [#11920](https://github.com/mixxxdj/mixxx/pull/11920)
  [#11961](https://github.com/mixxxdj/mixxx/pull/11961)
  [#12241](https://github.com/mixxxdj/mixxx/pull/12241)
  [#12394](https://github.com/mixxxdj/mixxx/pull/12394)
  [#12447](https://github.com/mixxxdj/mixxx/pull/12447)
  [#12425](https://github.com/mixxxdj/mixxx/pull/12425)
  [#12421](https://github.com/mixxxdj/mixxx/pull/12421)
  [#12799](https://github.com/mixxxdj/mixxx/pull/12799)
  [#12801](https://github.com/mixxxdj/mixxx/pull/12801)
  [#12800](https://github.com/mixxxdj/mixxx/pull/12800)
  [#12736](https://github.com/mixxxdj/mixxx/pull/12736)
  [#12692](https://github.com/mixxxdj/mixxx/pull/12692)
  [#12694](https://github.com/mixxxdj/mixxx/pull/12694)
  [#12695](https://github.com/mixxxdj/mixxx/pull/12695)
  [#12691](https://github.com/mixxxdj/mixxx/pull/12691)
  [#12693](https://github.com/mixxxdj/mixxx/pull/12693)
  [#12625](https://github.com/mixxxdj/mixxx/pull/12625)
  [#12627](https://github.com/mixxxdj/mixxx/pull/12627)
  [#12626](https://github.com/mixxxdj/mixxx/pull/12626)
  [#12577](https://github.com/mixxxdj/mixxx/pull/12577)
  [#13162](https://github.com/mixxxdj/mixxx/pull/13162)
  [#13163](https://github.com/mixxxdj/mixxx/pull/13163)
  [#13187](https://github.com/mixxxdj/mixxx/pull/13187)
  [#13217](https://github.com/mixxxdj/mixxx/pull/13217)
  [#13246](https://github.com/mixxxdj/mixxx/pull/13246)
  [#13232](https://github.com/mixxxdj/mixxx/pull/13232)
  [#13528](https://github.com/mixxxdj/mixxx/pull/13528)
  [#13595](https://github.com/mixxxdj/mixxx/pull/13595)


### Quoted Christmas songs

All I want for Christmas (Mariah Carey) | Santa Clause is Coming to Town (fi Bruce Springsteen) | Rockin' Around the Christmas Tree (Brenda Lee) | Cheer for the Elves (Gwen Stefani) | Presents for Christmas (Solomon Burke) | Last Christmas (Wham) | Driving home for Christmas (Chris Rea) | Christmas Will Break Your Heart (LCD Soundsystem) | Christmas Present (Andy Williams) | Rudolph, the Red-Nosed Reindeer (Johnny Marks) | Jingle Bells (traditional) | Santa Tell Me’ (Ariana Grande) | 8 Days Of Christmas (Destiny's Child) | Fairytale of New York (The Pogues & Kirsty MacColl) | Player’s Ball (Outkast) | I'll Be Home For Christmas (Bing Crosby) | underneath the Mistletoe (Kelly Clarkson) | Winter Wonderland (Bing Crosby) | Thank You Santa (Phineas and Ferb) | Feliz Navidad (José Feliciano) | Christmas Lights (Coldplay) | So this is Christmas (John Lennon) | Baby, It's Cold Outside (Ella Fitzgerald & Louis Armstrong) | Wonderful Christmas Time (Paul McCartney) | Light the Candles All Around the World (traditional)
