title: Mixxx 2.5 beta released
authors: Evelynne Veys
tags: 2.5, beta, release announcement
comments: yes
status: draft

#### Dear Mixxx-ers

Funny things happen in spring, birds start nesting and lay eggs, and so did the Mixxx developers.
A bit late for Easter but it is a magnificent giant gift filled with smaller gifts: Mixxx 2.5 beta!
You can find the details about the new version below.

#### Appeal

Before releasing 2.5 as the next stable release we need it to be tested thoroughly, something we can't do on our own.
After some time looking at the same release and searching for solutions we might forget miner bugs or problems.
That's why we need **YOU** to help us. The more people testing this Beta and reporting eventual bugs to the [bugtracker](https://github.com/mixxxdj/mixxx/issues), the faster the beta can be promoted to stable.
In case you're scared of messing up your neetly configured PC and losing your holy data is your Haloween-nightmare, read the new wiki article [safeguard your Mixxx Data](https://github.com/mixxxdj/mixxx/wiki).
It explains about making a timestamp-image, backing up your data, tips and tricks.
Please [join the Mixxx team](https://mixxx.org/get-involved/).
In Mixxx we trust.

#### Highlights

* In version 2.5 Mixxx steps up from QT 5 to QT 6 [QT-website](https://www.qt.io/product/qt6).
* Important for all controller mapping contributors: the introduction of the new handling of controller-mappings. Please give us feedback.


#### What's new / What's changed / What's corrected in 2.5 beta

You can download the new release from the [Download](https://mixxx.org/download/) page, the list of changes can be found in the [ChangeLog](https://github.com/mixxxdj/mixxx/blob/2.5/CHANGELOG.md)

##### Features

* Logging: Include timestamps in messages by default
  [#11861](https://github.com/mixxxdj/mixxx/pull/11861)
* MacOS: App proxy icon of the playing track to the window title
  [#12116](https://github.com/mixxxdj/mixxx/pull/12116)
* Add beats translate move ControlEncoder
  [#12376](https://github.com/mixxxdj/mixxx/pull/12376)
* New built-in effect: Glitch
  [#11329](https://github.com/mixxxdj/mixxx/pull/11329)
* Fullscreen toggle rework
  [#11566](https://github.com/mixxxdj/mixxx/pull/11566)
* Playlists: Update of playlist labels after adding tracks
  [#12866](https://github.com/mixxxdj/mixxx/pull/12866)
  [#12761](https://github.com/mixxxdj/mixxx/pull/12761)
* Tracks: Custom text color for played tracks (qss)
  [#12744](https://github.com/mixxxdj/mixxx/pull/12744)
  [#5911](https://github.com/mixxxdj/mixxx/pull/5911)
  [#12912](https://github.com/mixxxdj/mixxx/pull/12912)
* History: Show track count and duration in sidebar
  [#12811](https://github.com/mixxxdj/mixxx/pull/12811)
  [#12788](https://github.com/mixxxdj/mixxx/pull/12788)
* fixes around cratetablemodel, remove tracks + don't allow pasting tracks into locked playlists/crates or History
  [#12926](https://github.com/mixxxdj/mixxx/pull/12926)
* Tootips: Improve rate_up/down tooltips, pitch vs. speed
  [#12590](https://github.com/mixxxdj/mixxx/pull/12590)
* Shortkeys for track list management
  [#12020](https://github.com/mixxxdj/mixxx/pull/12020)
* Track menu: Rephrase "Reset" to "Clear"
  [#12955](https://github.com/mixxxdj/mixxx/pull/12955)
* PreviewDeckN,LoadSelectedTrackAndPlay toggles play/pause if the track is already loaded
  [#12920](https://github.com/mixxxdj/mixxx/pull/12920)
  [#9819](https://github.com/mixxxdj/mixxx/pull/9819)
* Added tooltip for expand/collapse samplers button.
  [#13005](https://github.com/mixxxdj/mixxx/pull/13005)
  [#12998](https://github.com/mixxxdj/mixxx/pull/12998)
* Add command line option --start-autodj to start Auto DJ immediately after Mixxx start.
  [#13017](https://github.com/mixxxdj/mixxx/pull/13017)
  [#10189](https://github.com/mixxxdj/mixxx/pull/10189)
* Allow to edit track title and artist directly within the decks via a delayed double-click
  [#11755](https://github.com/mixxxdj/mixxx/pull/11755)
* Preferences: Fix incorrect reboot required notification on preference updates
  [#13058](https://github.com/mixxxdj/mixxx/pull/13058)
* Effects: Add backend for Audio Unit (AU) plugins on macOS
  [#12112](https://github.com/mixxxdj/mixxx/pull/12112)
* Track menu, Remove from disk: stop and eject all affected decks
  [#13214](https://github.com/mixxxdj/mixxx/pull/13214)
* Require a minimum movement before initiating the drag&drop of tracks
  [#12903](https://github.com/mixxxdj/mixxx/pull/12903)
* Preferences: Add missing spacer in interface preference
  [#13094](https://github.com/mixxxdj/mixxx/pull/13094)
* Preferences: Fix fetching of soundcard sample rate
  [#11951](https://github.com/mixxxdj/mixxx/pull/11951)
  [#11949](https://github.com/mixxxdj/mixxx/pull/11949)
* Playlists: move tracks with Alt + Up/Down/PageUp/PageDown/Home/End
  [#13092](https://github.com/mixxxdj/mixxx/pull/13092)
  [#10826](https://github.com/mixxxdj/mixxx/pull/10826)
* Search: Add special BPM filters
  [#12072](https://github.com/mixxxdj/mixxx/pull/12072)
  [#8191](https://github.com/mixxxdj/mixxx/pull/8191)
* Search: Add "OR" search operator
  [#12061](https://github.com/mixxxdj/mixxx/pull/12061)
  [#8881](https://github.com/mixxxdj/mixxx/pull/8881)
* Add load point option 'First hotcue'
  [#12869](https://github.com/mixxxdj/mixxx/pull/12869)
  [#12740](https://github.com/mixxxdj/mixxx/pull/12740)
* Toggle the menubar with single Alt key press (auto hide)
  [#11526](https://github.com/mixxxdj/mixxx/pull/11526)
* Computer feature: add sidebar action "Refresh directory tree"
  [#12908](https://github.com/mixxxdj/mixxx/pull/12908)
* Library: Custom color for missing tracks
  [#12895](https://github.com/mixxxdj/mixxx/pull/12895)
* Library: Add feedback to directory operations (add, remove, relink)
  [#12436](https://github.com/mixxxdj/mixxx/pull/12436)
  [#10481](https://github.com/mixxxdj/mixxx/pull/10481)
* Library: Add support for scaling BPM by different ratios
  [#12934](https://github.com/mixxxdj/mixxx/pull/12934)
  [#9133](https://github.com/mixxxdj/mixxx/pull/9133)
* Library: Add ability to import external playlists as crates
  [#11852](https://github.com/mixxxdj/mixxx/pull/11852)
* Library: Add 'Shuffle playlist' sidebar action
  [#12498](https://github.com/mixxxdj/mixxx/pull/12498)
  [#6988](https://github.com/mixxxdj/mixxx/pull/6988)
* Beats: allow undoing the last BPM/beats change
  [#12954](https://github.com/mixxxdj/mixxx/pull/12954)
  [#12774](https://github.com/mixxxdj/mixxx/pull/12774)
  [#10138](https://github.com/mixxxdj/mixxx/pull/10138)
* Effects: Add Compressor
  [#1252](https://github.com/mixxxdj/mixxx/pull/1252)
* Add beatloop anchor to set and adjust loop from either start or end
  [#12745](https://github.com/mixxxdj/mixxx/pull/12745)
  [#13241](https://github.com/mixxxdj/mixxx/pull/13241)
* Handle not supported files when dragging to waveforms and spinnies
  [#13206](https://github.com/mixxxdj/mixxx/pull/13206)
* Add Rate Tap button
  [#12104](https://github.com/mixxxdj/mixxx/pull/12104)
* Store/restore regular loop when toggling rolling loops
  [#12475](https://github.com/mixxxdj/mixxx/pull/12475)
  [#8947](https://github.com/mixxxdj/mixxx/pull/8947)
* Add type toggle to cue popup
  [#13215](https://github.com/mixxxdj/mixxx/pull/13215)
* MIDI Input editor: allow selecting multiple Options
  [#12348](https://github.com/mixxxdj/mixxx/pull/12348)

##### Waveforms

* SlipMode waveform visual for RGB GLSL
  [#13002](https://github.com/mixxxdj/mixxx/pull/13002)
  [#13256](https://github.com/mixxxdj/mixxx/pull/13256)
* Show beats and time until next marker in the waveform
  [#12994](https://github.com/mixxxdj/mixxx/pull/12994)
* Waveforms: don't elide hotcue labels
  [#13219](https://github.com/mixxxdj/mixxx/pull/13219)
  [#10722](https://github.com/mixxxdj/mixxx/pull/10722)
* Waveforms: Allshader RGB, Filtered and Stacked Waveforms using textures for waveform data
  [#13151](https://github.com/mixxxdj/mixxx/pull/13151)
  [#12641](https://github.com/mixxxdj/mixxx/pull/12641)

##### Controller Mappings

* Pioneer DDJ-FLX4: Mapping improvements
  [#12842](https://github.com/mixxxdj/mixxx/pull/12842)
* Traktor S4 MK3: Add setting definition for
  [#12995](https://github.com/mixxxdj/mixxx/pull/12995)
* Traktor S4 MK3: Software mixer support and default pad layout customisation
  [#13059](https://github.com/mixxxdj/mixxx/pull/13059)

##### Controller Backend

* Send sysex to all handlers
  [#12827](https://github.com/mixxxdj/mixxx/pull/12827)
* Add control for showing a deck's track menu
  [#10825](https://github.com/mixxxdj/mixxx/pull/10825)
* Removed old examples HID keyboard and HID trackpad
  [#12977](https://github.com/mixxxdj/mixxx/pull/12977)
* Reduce log noise with HID device
  [#13010](https://github.com/mixxxdj/mixxx/pull/13010)
  [#13125](https://github.com/mixxxdj/mixxx/pull/13125)
* Allow controller mapping to discard polling
  [#12558](https://github.com/mixxxdj/mixxx/pull/12558)
* Add support for mapping user settings
  [#11300](https://github.com/mixxxdj/mixxx/pull/11300)
  [#13046](https://github.com/mixxxdj/mixxx/pull/13046)
  [#13057](https://github.com/mixxxdj/mixxx/pull/13057)
  [#13045](https://github.com/mixxxdj/mixxx/pull/13045)
* Registering MIDI Input Handlers From Javascript
  [#12781](https://github.com/mixxxdj/mixxx/pull/12781)
  [#13089](https://github.com/mixxxdj/mixxx/pull/13089)
* Add Track colour palette cycling controls track_color_next and track_color_prev to library, decks and samplers
  [#13066](https://github.com/mixxxdj/mixxx/pull/13066)
  [#12905](https://github.com/mixxxdj/mixxx/pull/12905)
* Add tempo lock control bpmlock to decks and samplers
  [#13041](https://github.com/mixxxdj/mixxx/pull/13041)
  [#13038](https://github.com/mixxxdj/mixxx/pull/13038)
  [#13199](https://github.com/mixxxdj/mixxx/pull/13199)
* Controller IO table: Fix display text for Action/control delegate
  [#13188](https://github.com/mixxxdj/mixxx/pull/13188)
* Tempo locking controls
  [#13041](https://github.com/mixxxdj/mixxx/pull/13041)
* Support for bulk devices on Windows and Mac
  [#13008](https://github.com/mixxxdj/mixxx/pull/13008)
* Add Track colour palette cycling controls for decks
  [#13066](https://github.com/mixxxdj/mixxx/pull/13066)
* Registering MIDI Input Handlers From Javascript
  [#12781](https://github.com/mixxxdj/mixxx/pull/12781)
  [#13089](https://github.com/mixxxdj/mixxx/pull/13089)

##### Library

* Track widgets: set show_track_menu only for main decks
  [#12978](https://github.com/mixxxdj/mixxx/pull/12978)
* Track menu: add star rating
  [#12700](https://github.com/mixxxdj/mixxx/pull/12700)
  [#10652](https://github.com/mixxxdj/mixxx/pull/10652)
* Playlists: move tracks with Alt + Up/Down/PageUp/PageDown/Home/End
  [#13092](https://github.com/mixxxdj/mixxx/pull/13092)
  [#10826](https://github.com/mixxxdj/mixxx/pull/10826)

##### Skins

* LateNight: Merge vinyl control toggle and status light
  [#12947](https://github.com/mixxxdj/mixxx/pull/12947)
  [#10192](https://github.com/mixxxdj/mixxx/pull/10192)

##### Experimental QML Skin

* Add Experimental QML Skin that can be tested via the --qml command line option
  [#13152](https://github.com/mixxxdj/mixxx/pull/13152)
* Fix type error in Slider.qml
  [#11423](https://github.com/mixxxdj/mixxx/pull/11423)
* Allow switching between legacy and new QML UI with command arg
  [#12139](https://github.com/mixxxdj/mixxx/pull/12139)
* Add PlayerProxy missing current track when created after loading
  [#12559](https://github.com/mixxxdj/mixxx/pull/12559)
* add qt6-qpa-plugins to dependencies
  [#12549](https://github.com/mixxxdj/mixxx/pull/12549)
* fix(qml): Improve knobs by applying selective 4xMSAA on the Arc shape
  [#12541](https://github.com/mixxxdj/mixxx/pull/12541)
* Add QML interceptor to auto reload on file change
  [#12795](https://github.com/mixxxdj/mixxx/pull/12795)
  [#12844](https://github.com/mixxxdj/mixxx/pull/12844)
* Add multi-sampling settings for QML
  [#12546](https://github.com/mixxxdj/mixxx/pull/12546)
  [#12794](https://github.com/mixxxdj/mixxx/pull/12794)
  [#12536](https://github.com/mixxxdj/mixxx/pull/12536)
  [#13058](https://github.com/mixxxdj/mixxx/pull/13058)
* Install qml module on Windows
  [#12604](https://github.com/mixxxdj/mixxx/pull/12604)
* Add scrolling waveforms
  [#3967](https://github.com/mixxxdj/mixxx/pull/3967)
  [#13009](https://github.com/mixxxdj/mixxx/pull/13009)
* fix(QML): handle case where Waveform data is missing
  [#13009](https://github.com/mixxxdj/mixxx/pull/13009)
* fix: allow missing COs on QML component
  [#13011](https://github.com/mixxxdj/mixxx/pull/13011)
* Initialize CmdlineArgs::m_qml
  [#13152](https://github.com/mixxxdj/mixxx/pull/13152)

##### Update to Qt6

* Qt6 switch
  [#11892](https://github.com/mixxxdj/mixxx/pull/11892)
* CMakeLists: Default QT6 to ON
  [#11934](https://github.com/mixxxdj/mixxx/pull/11934)
* Build with Qt6 and optionally with QML
  [#11608](https://github.com/mixxxdj/mixxx/pull/11608)
* Qt6: Use constInsert() template
  [#11847](https://github.com/mixxxdj/mixxx/pull/11847)
* Qt6 prepare
  [#11863](https://github.com/mixxxdj/mixxx/pull/118863)
* DlgAbout: Add Qt version to the dialog
  [#11862](https://github.com/mixxxdj/mixxx/pull/11862)
* CMakeLists: Fix QT_TRANSLATION_FILE path for Qt 6
  [#11880](https://github.com/mixxxdj/mixxx/pull/11880)
* LibraryControl: Enable control inputs for Qt 6
  [#11877](https://github.com/mixxxdj/mixxx/pull/11877)
* Fix wrong Windows buildenv name and missing Qt6 switch for non CI builds
  [#11895](https://github.com/mixxxdj/mixxx/pull/11895)
* WWidget: Disable touch events on macOS (fixing trackpad issues on Qt 6)
  [#11870](https://github.com/mixxxdj/mixxx/pull/11870)
* Install libjpeg-turbo::jpeg to fix cover display with Qt6
  [#11922](https://github.com/mixxxdj/mixxx/pull/11922)
* Skins: Remove border: 0px from sidebar item styling
  [#11970](https://github.com/mixxxdj/mixxx/pull/11970)
  [#11957](https://github.com/mixxxdj/mixxx/pull/11957)
* Introduce wrapper for non const iterators for erase and insert
  [#12201](https://github.com/mixxxdj/mixxx/pull/12201)
* Skins: Fix checkbox styling on Qt 6
  [#12050](https://github.com/mixxxdj/mixxx/pull/12050)
* Fix Qt6/QML build
  [#12255](https://github.com/mixxxdj/mixxx/pull/12255)
* Fix track color background with Qt6
  [#12380](https://github.com/mixxxdj/mixxx/pull/12380)
* multi-line delegate: fix bg color, Qt6 on Linux
  [#12478](https://github.com/mixxxdj/mixxx/pull/12478)
* Revert "BaseTrackPlayer: Remove references to WaveformWidgetRenderer when using Qt6"
  [#12342](https://github.com/mixxxdj/mixxx/pull/12342)
* Fix Tango waveform splitter
  [#12939](https://github.com/mixxxdj/mixxx/pull/12939)
* Fix: Replace deprecated qAsConst with std::as_const
  [#13028](https://github.com/mixxxdj/mixxx/pull/13028)
* Fix Drag'n'drop: avoid unintended drag on hover (WTrackProperty, WCoverArt etc.)
  [#13035](https://github.com/mixxxdj/mixxx/pull/13035)
  [#13033](https://github.com/mixxxdj/mixxx/pull/13033)
* Fix ambiguous overload error due to native qDebug impl for std::optional
  [#12981](https://github.com/mixxxdj/mixxx/pull/12981)
* Fix 'selected click' bug
  [#12488](https://github.com/mixxxdj/mixxx/pull/12488)
* Tango: Fix rate range label position
  [#13242](https://github.com/mixxxdj/mixxx/pull/13242)

##### Experimental iOs support

* CMakeLists: Support building for iOS
  [#12672](https://github.com/mixxxdj/mixxx/pull/12672)
* DlgPrefInterface: Disable tooltips on iOS by default
  [#12689](https://github.com/mixxxdj/mixxx/pull/12689)
* SoundManager: Set up AVAudioSession on iOS
  [#12714](https://github.com/mixxxdj/mixxx/pull/12714)
* SoundManager: Use correct PortAudio backend on iOS
  [#12716](https://github.com/mixxxdj/mixxx/pull/12716)
* DesktopHelper: Add openUrl abstraction to support iOS
  [#12698](https://github.com/mixxxdj/mixxx/pull/12698)
* iOS packaging: Add Info.plist, launch screen and app icon
  [#12676](https://github.com/mixxxdj/mixxx/pull/12676)
* CmdlineArgs: Move config directory to a user-accessible location on iOS
  [#12688](https://github.com/mixxxdj/mixxx/pull/12688)

##### Experimental WebAssembly support

* CMakeLists: Add support for targeting Emscripten/WebAssembly
  [#12918](https://github.com/mixxxdj/mixxx/pull/12918)
* CMakeLists: Emit better errors for exotic target platforms
  [#12910](https://github.com/mixxxdj/mixxx/pull/12910)
* Build: Add PORTMIDI flag for compiling with(out) PortMidi
  [#12913](https://github.com/mixxxdj/mixxx/pull/12913)
* DesktopHelper: Compile out process-spawning on WASM too
  [#12916](https://github.com/mixxxdj/mixxx/pull/12916)
* MixxxApplication: Use QWasmIntegrationPlugin when targeting WebAssembly
  [#12915](https://github.com/mixxxdj/mixxx/pull/12915)
* CMakeLists: Enable asyncify when targeting WASM
  [#12921](https://github.com/mixxxdj/mixxx/pull/12921)
* Resources: Bundle resources for preloading when targeting Emscripten/WASM
  [#12922](https://github.com/mixxxdj/mixxx/pull/12922)
* CMakeLists: Add WASM_ASSERTIONS option
  [#12931](https://github.com/mixxxdj/mixxx/pull/12931)
* VersionStore: Recognize Emscripten/WebAssembly
  [#12940](https://github.com/mixxxdj/mixxx/pull/12940)
* OpenGLWindow: Fix sizing on Wasm by setting Qt::FramelessWindowHint
  [#12945](https://github.com/mixxxdj/mixxx/pull/12945)
* CMakeLists: Require WebGL 2.0 when building for Wasm
  [#12952](https://github.com/mixxxdj/mixxx/pull/12952)
* ScreenSaverHelper: Add no-op implementation for WASM
  [#12930](https://github.com/mixxxdj/mixxx/pull/12930)
* SSE: Check !defined(__EMSCRIPTEN__) where intrinsics are unavailable on WASM
  [#12917](https://github.com/mixxxdj/mixxx/pull/12917)

##### Target support

* Lenient taglib 2.0 guard
  [#12793](https://github.com/mixxxdj/mixxx/pull/12793)
* Tools: Add rpm_buildenv.sh for building on Fedora
  [#13069](https://github.com/mixxxdj/mixxx/pull/13069)
* README: Recommend running buildenvs over sourcing them on Linux
  [#13071](https://github.com/mixxxdj/mixxx/pull/13071)
* FindSndFile: Link mpg123 in static builds
  [#13087](https://github.com/mixxxdj/mixxx/pull/13087)

##### Misc Refactorings

* Add missing <Qt> include in defs.h
  [#11348](https://github.com/mixxxdj/mixxx/pull/11348)
* engine: Minor refactor to prefer simplified ranged-for-loop
  [#11234](https://github.com/mixxxdj/mixxx/pull/11234)
* Delete unused EngineFilter
  [#11559](https://github.com/mixxxdj/mixxx/pull/11559)
* AnalyzerWaveform: Fix commented out code
  [#11561](https://github.com/mixxxdj/mixxx/pull/11561)
* Remove usage of ControlObject::getControl
  [#11643](https://github.com/mixxxdj/mixxx/pull/11643)
* Fixed unnecessary transfer of the ownership before release which returns the pointer itself
  [#11726](https://github.com/mixxxdj/mixxx/pull/11726)
* add ConfigObject::get-/setValue<EnumType>
  [#11883](https://github.com/mixxxdj/mixxx/pull/11883)
* ci: Enable WARNINGS_FATAL on macOS, too
  [#11905](https://github.com/mixxxdj/mixxx/pull/11905)
* Refactor timers 
  [#11807](https://github.com/mixxxdj/mixxx/pull/11905) 2nd try
  [#11850](https://github.com/mixxxdj/mixxx/pull/11850)
* Use mixxx::audio::ChannelCount type instead of int/unsigned char/etc.
  [#11941](https://github.com/mixxxdj/mixxx/pull/11941)
* refactor(util/timer): cleanup includes
  [#11937](https://github.com/mixxxdj/mixxx/pull/11937)
* Use SampleRate type consistently
  [#11904](https://github.com/mixxxdj/mixxx/pull/11904)
* CMakeLists: Match arbitrary arm64-osx triplets
  [#11933](https://github.com/mixxxdj/mixxx/pull/11933)
* Alex/reduce sample buffer memory usage
  [#11988](https://github.com/mixxxdj/mixxx/pull/11988)
* Fix clazy issues on main
  [#12028](https://github.com/mixxxdj/mixxx/pull/12028)
* Tidy and modernize SampleBuffer
  [#11987](https://github.com/mixxxdj/mixxx/pull/11987)
* Refactor(parented_ptr): make trivially destructible in release mode, delete move operations
  [#11981](https://github.com/mixxxdj/mixxx/pull/11981)
* Labeler: Add more labels to the auto-labeler
  [#12106](https://github.com/mixxxdj/mixxx/pull/12106)
* macOS packaging: Enable app sandbox in ad-hoc-packaged (i.e. non-notarized) bundles too
  [#12101](https://github.com/mixxxdj/mixxx/pull/12101)
* FindPortMidi: Link ALSA in static builds on Linux
  [#12292](https://github.com/mixxxdj/mixxx/pull/12292)
  [#12291](https://github.com/mixxxdj/mixxx/pull/12291)
* privat generated ui headers
  [#12060](https://github.com/mixxxdj/mixxx/pull/12060)
  [#11407](https://github.com/mixxxdj/mixxx/pull/11407)
* ci: workaround runner-image issue
  [#12233](https://github.com/mixxxdj/mixxx/pull/12233)
* FindLibudev: Link hidapi and libusb with libudev in static builds on Linux
  [#12294](https://github.com/mixxxdj/mixxx/pull/12294)
* FindVorbis: Link ogg in static builds
  [#12297](https://github.com/mixxxdj/mixxx/pull/12297)
* MixxxApplication: Support linking Qt statically on Linux
  [#12284](https://github.com/mixxxdj/mixxx/pull/12284)
* FindSleef: Use OpenMP in static builds
  [#12295](https://github.com/mixxxdj/mixxx/pull/12295)
* Happy New Year 2024!
  [#12486](https://github.com/mixxxdj/mixxx/pull/12486)
* fix/History: remove obsolete placeholder playlists
  [#12494](https://github.com/mixxxdj/mixxx/pull/12494)
* Add missing Taglib dependency
  [#12830](https://github.com/mixxxdj/mixxx/pull/12830)
* fix: typo ;)
  [#12726](https://github.com/mixxxdj/mixxx/pull/12726)
* refactor: Avoid temporary qlist allocation on midi sysex receive
  [#12843](https://github.com/mixxxdj/mixxx/pull/12843)
* Labeler: Add qml to labeler config
  [#12911](https://github.com/mixxxdj/mixxx/pull/12911)
* WTrackMenu: Add missing wcoverartlabel.h include
  [#12924](https://github.com/mixxxdj/mixxx/pull/12924)
* Fix clazy complains and naming
  [#12935](https://github.com/mixxxdj/mixxx/pull/12935)
* src/library: Sort files into sub-directories
  [#12956](https://github.com/mixxxdj/mixxx/pull/12956)
* CMakeLists: Fix deduplication trap with --preload-file
  [#12944](https://github.com/mixxxdj/mixxx/pull/12944)
* Add CI runner that allows cleaning up the download server
  [#12957](https://github.com/mixxxdj/mixxx/pull/12957)
* Refactor FFmpeg soundsource to allow other soundsource to inherit it
  [#13042](https://github.com/mixxxdj/mixxx/pull/13042)
* Code Style: Add branches around single line blocks.
  [#13097](https://github.com/mixxxdj/mixxx/pull/13097)
* fix: add missing member in copy ctor
  [#13229](https://github.com/mixxxdj/mixxx/pull/13229)
* Refactor/preferences enums
  [#12798](https://github.com/mixxxdj/mixxx/pull/12798)
* Update to latest vcpkg dependencies
  [#11649](https://github.com/mixxxdj/mixxx/pull/11649)
  [#12512](https://github.com/mixxxdj/mixxx/pull/12512)
  [#12067](https://github.com/mixxxdj/mixxx/pull/12067)
  [#12898](https://github.com/mixxxdj/mixxx/pull/12989)
  [#13155](https://github.com/mixxxdj/mixxx/pull/13155)
* GitHub actions updates
  [#11544](https://github.com/mixxxdj/mixxx/pull/11544)
  [#11508](https://github.com/mixxxdj/mixxx/pull/11508) 
  [#11487](https://github.com/mixxxdj/mixxx/pull11487/) 
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
