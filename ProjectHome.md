<a href='http://qt.nokia.com/qt-in-use/ambassadors/showcase'><img width='150' align='right' height='150' src='http://voicetogoog.googlecode.com/svn/wiki/qt_ambassador_logo.png' /></a>
<p align='center'><font size='5'><b>VoiceToGoog</b></font></p>
<p align='center'><b>Niels P. Mayer ( <a href='http://www.nielsmayer.com'>http://www.nielsmayer.com</a> )</b></p>

<p align='left'><img width='250' align='left' height='333' src='http://27.media.tumblr.com/tumblr_lvg2tv1LYN1qh56plo1_500.jpg' /></p>



<blockquote><p align='justify'>VoiceToGoog helps people organize their voice thoughts using text annotation automatically provided by voice-to-text technology. All notes are time and location stamped to provide easy context-sensitivity -- allowing visual browsing of one's notes, activities (external program launch) by both time and location. The browsing experience is augmented by map-view mashups indicating where given speech/note/activity took place. As a utility application, VoiceToGoog is a primary enabler of mobile literacy because it allows the user the ability to use voice instead of typing and can even read back the transcribed text. Of course you can do all the expected things like using voice for Google-search, YouTube-search, map-search, or e-mail on the transcribed contents, or using the spoken phone number, or contact name, to call or email that contact.</p></blockquote>

<p align='center'><a href='http://www.youtube.com/watch?feature=player_embedded&v=oEYMsrA_8gY' target='_blank'><img src='http://img.youtube.com/vi/oEYMsrA_8gY/0.jpg' width='854' height=480 /></a></p>
<p align='center'><a href='http://www.youtube.com/watch?feature=player_embedded&v=OCNwRXQFcdw' target='_blank'><img src='http://img.youtube.com/vi/OCNwRXQFcdw/0.jpg' width='854' height=480 /></a></p>

<p align='center'><img src='http://voicetogoog.googlecode.com/svn/wiki/voicetogoog-embedded-webserver-exhibit-search.png' width='854' height='480' /></p>
<p align='center'><b>Coming soon... <a href='http://www.simile-widgets.org/exhibit/'>Simile-Widgets Exhibit</a>-based Embedded Webserver Faceted Search</b></p><br />
<p align='center'><img src='http://voicetogoog.googlecode.com/svn/wiki/voicetogoog-embedded-webserver-exhibit-mapview.png' width='854' height='480' /></p>
<p align='center'><b>Coming soon... <a href='http://www.simile-widgets.org/exhibit/'>Simile-Widgets Exhibit</a>-based Embedded Webserver Map-View</b></p><br />
<p align='center'><img src='http://voicetogoog.googlecode.com/svn/wiki/voicetogoog-embedded-webserver-exhibit-timeline.png' width='854' height='480' /></p>
<p align='center'><b>Coming soon... <a href='http://www.simile-widgets.org/exhibit/'>Simile-Widgets Exhibit</a>-based Embedded Webserver Timeline-View</b></p><br />
<p align='center'><img src='http://voicetogoog.googlecode.com/svn/wiki/voicetogoog-embedded-webserver-exhibit-calendarview.png' width='854' height='480' /></p>
<p align='center'><b>Coming soon... <a href='http://www.simile-widgets.org/exhibit/'>Simile-Widgets Exhibit</a>-based Embedded Webserver Calendar-View</b></p><br />


## Now available for free download at store.nokia.com! ##

VoiceToGoog 0.3.0 has been released for free download at http://store.nokia.com/content/195998 for the amazing [Linux/!MeeGo-based](http://harmattan-dev.nokia.com/docs/library/html/guide/html/Developer_Library_MeeGo_1.2_Harmattan_Developer_Library.html) [Nokia N9](http://swipe.nokia.com) as well as the [Nokia N950 developer handset](http://www.engadget.com/2011/06/21/nokias-n950-developer-meego-handset-gets-official-4-inch-displ/).

See also:
<ul>
<li><a href='http://my-meego.com/downloads/search.php?name=VoiceToGoog'>http://my-meego.com/downloads/search.php?name=VoiceToGoog</a></li>
<li><a href='http://www.mwkn.net/2011/45/apps.html'>http://www.mwkn.net/2011/45/apps.html</a></li>
<li><a href='http://nokia.hdblog.it/2011/11/04/voicetogoog-il-riconoscimento-vocale-di-google-multifunzione-per-meego-harmattan-video/'>http://nokia.hdblog.it/2011/11/04/voicetogoog-il-riconoscimento-vocale-di-google-multifunzione-per-meego-harmattan-video/</a></li>
<li><a href='http://hassantahir.com/2011/11/voicetogoog-speech-recognition-multipurpose-meego-harmattan-google/'>http://hassantahir.com/2011/11/voicetogoog-speech-recognition-multipurpose-meego-harmattan-google/</a></li>
</ul>

## Releases ##

voicetogoog (0.3.0) stable; urgency=high

  * VoiceToGoog 0.3.0: Fourth release to http://store.nokia.com/content/195998 ( see also http://code.google.com/p/voicetogoog/ ).
  * /opt/voicetogoog/qml/voicetogoog/main\_harmattan.qml          : Launches on Harmattan platform, using a toplevel PageStackWindow element, which enables support for portrait mode and automatic rotation into landscape, as well as other Harmattan platform integration features. For example, the fullscreen() method toggles visibility of the Harmattan status-bar; note that VoiceToGoog will continue to start-up fullscreen on Harmattan -- now, however, deselecting "Fullscreen" works correctly and reorients the status-bar appropriately during rotation. Note that the size of the main window is reduced by 35 pixels to compensate for the size of the status-bar when not in full screen mode -- '35' may not be correct. Couldn't find a system constant representing this value.
  * /opt/voicetogoog/qml/voicetogoog/main\_linux.qml              : Launches on Linux/MeeGo platform, using generic QML interface provided by using a toplevel 'Rectangle' element. Portrait mode on Linux desktop is dynamically enabled when the window is resized to be longer than it is wide. On the desktop, the fullscreen() method makes the app go full-screen on Linux desktops, and displays without titlebar on MeeGo Netbook; the app starts as a regular sized window on the desktop  -- to go fullscreen, user should select "Fullscreen" option in the menu.
  * /opt/voicetogoog/qml/voicetogoog/main\_symbian.qml            : Launches on Symbian platform. This is a placeholder for the future, in case someone submits code to integrate this platform, or Nokia sends me a 701 ( http://www.allaboutsymbian.com/reviews/item/13589_Nokia_701_part_1-hardware_OS_a.php ) to do it myself.
  * /opt/voicetogoog/qml/voicetogoog/VoiceToGoog.qml             : The VoiceToGoog QML element, a 'Rectangle' subclass, implements majority of platform-independent code comprising the application; its caller, `main_{linux,harmattan,symbian}.qml`, is where any platform dependencies should be.
  * /opt/voicetogoog/qml/voicetogoog/UtterDelegate.qml           : The details-view supports portrait mode, hiding some information which doesn't fit, and dynamically re-exposing that information when rotated into landscape. Now using 'utteranceText.paintedHeight' to accurately determine height of varying length of transcription contents. The value is forced to recalculate on reorientation through a declarative dependency (with invariant result) on a size-change in window.height and window.width; If no location information, the details view shows the transcription confidence percentage; if location information present, drop confidence percentage and location details (e.g. "range\_interpolated" or "rooftop").
  * /opt/voicetogoog/qml/voicetogoog/VoiceToGoog.qml             : The record, language-menu, toplevel-menu, and pause buttons are resized for portrait mode display. Some of the state-based text instructions in the buttons is removed in portrait mode because it won't fit.
  * /opt/voicetogoog/qml/voicetogoog/MenuDelegate.qml            : Menu entries containing parenthetical comments delimited by "[" have the comment text removed from display in portrait mode because they won't fit. The details are dynamically added back in landscape mode.
  * /opt/voicetogoog/qml/voicetogoog/component/.qml             : All dialogs and other open-source components in this directory now properly support dynamic resizing on orientation change.
  * /opt/voicetogoog/qml/voicetogoog/component/ModalTextEdit.qml : The "Edit Selection" functionality contains a dialog with four buttons in Landscape mode -- the "copy to clipboard" button is removed from view in portrait mode because it won't fit. Cleanup implementation and rationalize code that pops/lowers VKB.
  * /opt/voicetogoog/qml/voicetogoog/VoiceToGoog.qml             : In portrait mode, Comp.SplashScreen instance is invoked with gfx/splash\_screen\_portrait.png (stretched from original landscape-mode gfx/splash\_screen.png, should be redone with more legible text).
  * /opt/voicetogoog/qml/voicetogoog/scripts/commands.js         : URLs presented in dialogs use more legible _ACTIVE\_TEXT\_COLOR to highlight URLs -- CMD.openUrlExternally() and CMD.aboutVoicetogoog() use_RICHTEXT\_STYLESHEET\_PREAMBLE _RICHTEXT\_STYLESHEET\_APPENDIX to bracket displayed text.
  * /opt/voicetogoog/qml/voicetogoog/landmarkmap/Slider.qml      : In map-vew, this new implementation correctly repositions the slider on rotation. Updated/merged with code from a newer Nokian implementation of original source.
  * /opt/voicetogoog/qml/voicetogoog/scripts/commands.js         : CMD.voicetogoogExternalIssueReport() and CMD.voicetogoogExternalFeatureRequest() both invoke CMD.externalIssueReportLabels() to pre-fill the online issue-tracker labels with information extracted from following: 'appLang' 'appRegion' 'recognizerLanguageModel.currentISO639Language()' 'desktop.width' 'desktop.height' 'isOnline' 'Controller.isHarmattan'. Updated templates associated with http://code.google.com/p/voicetogoog/issues/entry?template=Defect%20report%20from%20user and http://code.google.com/p/voicetogoog/issues/entry?template=Feature%20Request to not ask user to paste this information from the terminal as that isn't going to happen for most users.
  * /opt/voicetogoog/qml/voicetogoog/MenuModel.qml               : Added 'Help Using VoiceToGoog' entry and associated CMD.voicetogoogExternalHelp() which launches http://code.google.com/p/voicetogoog/wiki/!VoiceToGoog_Help (TBD/WIP).._

> -- Niels Mayer  Wed, 30 Nov 2011 18:30:00 -0700

> voicetogoog (0.2.1) stable; urgency=high

  * VoiceToGoog 0.2.1: Actual second release to http://store.nokia.com/content/195998 ( see also http://code.google.com/p/voicetogoog/ ).
  * Fixed regression introduced in 0.2.0 CMD.selectAllFromStart(), CMD.selectAllFromEnd(), CMD.selectUntranscribedEntries() which broke "playlisting" of selection for playback or upload.
  * Increase efficiency of CMD.selectAllFromStart(), CMD.selectAllFromEnd(), CMD.selectUntranscribedEntries(); switch to details view to prevent all the seleccted map items text from overlaying and making a mess on the display, plus it's slow if there are hundreds of map items.
  * Fixed issue with accidental gestures above the menus being passed to underlying map or details view (causing accidental scrolling or selection) while either of the menus are up. The menu "Dimmer" now takes up full screen, with stacking order above the views but below the record/pause/menu buttons.
  * Modified map view slider-button have same visual appearance as other buttons -- transparent.
  * Work-around issue with YouTube search causing VoiceToGoog to fail validation for China in Nokia's store because of functionality, such as YouTube, that is unavailable in China. Work-around by removing functionality that doesn't work in China, based on detecting the presence of locale "zh-CN." Language-switching GUI introduced in 0.2.0 allows users to select "zh-CN" via the language menu. Other "zh" locales enable functionality disabled for "zh-CN." (Correct solution is detailed in http://code.google.com/p/voicetogoog/issues/detail?id=2 "Allow regional and/or user customization of external application launchers")

> -- Niels Mayer  Fri, 11 Nov 2011 21:00:00 -0700

> voicetogoog (0.2.0) stable; urgency=high

  * VoiceToGoog 0.2.0: Aborted second release to http://store.nokia.com/content/195998 ( see also http://code.google.com/p/voicetogoog/ ).
  * Adds language selection menu/button/icon with flag and language-code display, showing current recognition language and clarifying which language is recognized by default at application startup based on user's locale.
  * Locales not matching existing voice recognition languages default to British English (en-GB) with the language selection button showing a UK flag to indicate default input language to be used.
  * Switch language locales on-the-fly via GUI for voice-to-text languages British English (en-GB), Amercian English (en-US), Mandarin Chinese (zh-guoyu,zh-CN), Japanese (ja), French (fr), Italian (it), German (de). Spanish (es), Korean (ko).
  * New voice-to-text support and language switching for Australian English (en-AU), Indian English (en-IN), New Zealand English (en-NZ), South African English (en-ZA), Latin American Spanish (es-419), Indonesian (ind), Malaysian (zsm), Mandarin for Taiwan (zh-TW), Turkish (tr), Russian (ru), Czech (cs), Polish (pl), Brazilian Portuguese (pt-BR), Dutch (nl), Afrikaans (af), and Zulu (zu).
  * For some new languages, Latin American Spanish (es-419), Indonesian (ind), Malaysian (zsm), Zulu (zu), text-to-speech output doesn't work; voice-recogniztion language for English dialects doesn't produce the same accent on text-to-speech.
  * For more info on languages supported by Google's services, see http://www.google.com/support/mobile/bin/answer.py?hl=en&answer=165480 http://www.google.com/support/mobile/bin/answer.py?answer=169105#voice http://www.google.com/support/mobile/bin/answer.py?answer=169105#tts http://googleresearch.blogspot.com/2010/06/google-search-by-voice-now-available-in.html http://googleresearch.blogspot.com/2010/06/google-launches-korean-voice-search.html http://googleresearch.blogspot.com/2010/12/google-launches-cantonese-voice-search.html http://googleresearch.blogspot.com/2011/03/word-of-mouth-introducing-voice-search.html
  * Various minor fixes, changes, and frobbings.

> -- Niels Mayer   Thu, 10 Nov 2011 05:30:00 -0700

> voicetogoog (0.1.0) stable; urgency=high

  * VoiceToGoog 0.1.0: First release of voicetogoog.
  * Supports language locales English (en), Mandarin Chinese (zh), Japanese (ja), French (fr), Italian (it), German (de). Spanish (es), Korean (ko).
  * en-US and en-CA both default to "en-US" locale; Britain and English	locales not matching above default to "en-GB" locale.
  * More features, usability/UI improvements, better Harmattan UX next release.

> -- Niels Mayer  Fri, 28 Oct 2011 18:00:00 -0700

<a href='Hidden comment: 
!VoiceToGoog (0.1.0) stable; urgency=high
* First release of !VoiceToGoog.
* Supports speech input and output in language locales English (en), Mandarin Chinese (zh), Japanese (ja), French (fr), Italian (it), German (de). Spanish (es), Korean (ko).
* en-US and en-CA both default to "en-US" locale; British and locales not matching above all default to "en-GB" locale.
* More features, usability/UI improvements, better Harmattan UX next release.
'></a>

## Screenshots of Version 0.2.0 ##
<p align='center'><img src='http://nielsmayer.com/voicetogoog/voicetogoog-0.2.0-harmattan-mapview.png' /></p>
<p align='center'><b>Map-View</b></p><br />
<p align='center'><img src='http://nielsmayer.com/voicetogoog/voicetogoog-0.2.0-harmattan-detailview.png' /></p>
<p align='center'><b>Details View</b></p><br />
<p align='center'><img src='http://nielsmayer.com/voicetogoog/voicetogoog-0.2.0-harmattan-menuview.png' /></p>
<p align='center'><b>Menu View</b></p><br />
<p align='center'><img src='http://nielsmayer.com/voicetogoog/voicetogoog_harmattan_recording.png' /></p>
<p align='center'><b>Recording a new voice note, prior to transcription (v 0.1.0)</b></p><br />

## Screenshots of Version 0.2.1 ##

<p align='center'><img src='http://nielsmayer.com/voicetogoog/voicetogoog-0.2.1-harmattan-russian.png' /></p>
<p align='center'><b>Details View, Russian Selected</b></p><br />
<p align='center'><img src='http://nielsmayer.com/voicetogoog/voicetogoog-0.2.1-harmattan-polish-turkish.png' /></p>
<p align='center'><b>Details View, Polish Selected (also showing some Romanian words understood by selecting Turkish language comprehension).</b></p><br />
<p align='center'><img src='http://nielsmayer.com/voicetogoog/voicetogoog-0.2.1-harmattan-langmenu.png' /></p>
<p align='center'><b>English dialect selection in Language Menu</b></p><br />

<a href='Hidden comment: 
== Screenshots of Version 0.1.0 ==

<p align="center">http://nielsmayer.com/voicetogoog/voicetogoog_harmattan_mapview.png

Unknown end tag for &lt;/p&gt;


<p align="center">http://nielsmayer.com/voicetogoog/voicetogoog_harmattan_detailview.png

Unknown end tag for &lt;/p&gt;


<p align="center">http://nielsmayer.com/voicetogoog/voicetogoog_harmattan_menuview1.png

Unknown end tag for &lt;/p&gt;


<p align="center">http://nielsmayer.com/voicetogoog/voicetogoog_harmattan_menuview2.png

Unknown end tag for &lt;/p&gt;


<p align="center">http://nielsmayer.com/voicetogoog/voicetogoog_harmattan_menuview3.png

Unknown end tag for &lt;/p&gt;


<p align="center">http://nielsmayer.com/voicetogoog/voicetogoog_harmattan_menuview4.png

Unknown end tag for &lt;/p&gt;


<p align="center">http://nielsmayer.com/voicetogoog/voicetogoog_harmattan_menuview5.png

Unknown end tag for &lt;/p&gt;


<p align="center">http://nielsmayer.com/voicetogoog/voicetogoog_harmattan_menuview6.png

Unknown end tag for &lt;/p&gt;


<p align="center">http://nielsmayer.com/voicetogoog/voicetogoog_harmattan_recording.png

Unknown end tag for &lt;/p&gt;


'></a>

## Future ##

The platform tools, such as video/photo capture tools, may offer options to embed geolocation  information with their media. VoiceToGoog would make use of this information in enabling voice-and-location annotation of arbitrary media/document items on the handset. This is achieved via [Gallery/Tracker](http://doc.qt.nokia.com/qtmobility/qml-gallery.html) integration to allow voice-to-text annotation of geotagged photos and videos. Geotagged media displays similar to VoiceToGoog's audio notes in the map-view, but with a different icon indicative of media type, such as audio, video, photo, etc. This would be a significant improvement in the  http://code.google.com/p/ytd-meego/wiki/CitizenJournalismWithYoutubeDirectForMeego concept -- in terms of selecting and reporting on media with external audio notes and their transcribed textual representation. In practice, the selected map-region plots captured media-files and their associated geolocation info by searching via http://doc.qt.nokia.com/qtmobility-1.2/qml-gallerycontainsfilter.html and looking up geotag information from http://doc.qt.nokia.com/qtmobility-1.2/qml-documentgalleryitem.html#properties-prop . These "media landmarks" can then be associated with any number of VoiceToGoog audio annotations, which would show up as annotations located in association with the media, along with the traditional VoiceToGoog central-data-structure that captures an accurate timestamp and Geotag of each speech utterance. The transcribed text is one piece of attached data. The other would be the attachment to a given task (which is also a first-class data-item with its own graphical representation and associated time/location data). And another would be attachments to  these aforementioned "Document Gallery" objects provided by platform. By using a centralized and multifarious data-type, eased by the use of dynamic language JavaScript/QML, one thus can achieve arbitrary associations of these multifarious data-items that are the central data-type of VoiceToGoog.

It is a testament to the Harmattan/MeeGo platform that small amounts of application-level coding can create a big and useful feature, by leveraging [QML qsparql capabilities of the Qt Framework](http://blogs.kde.org/node/4340) and a well constructed [QSPARQL query](http://people.igalia.com/aperez/files/qsparql.pdf) and the [SLO Ontology for Locations](http://git.gnome.org/browse/tracker/tree/data/ontologies/92-slo.ontology). For example, the following shell command, issued via SSH, lists all the location-tagged photos and videos I've taken on the Nokia N950, which I'd like to be able to plot and voice-annotate on the VoiceToGoog map mashup:

```
~ $ tracker-sparql -q 'SELECT nie:url(?u) ?cty ?cry {                         \
                                                     ?u slo:location          \
                                                     [ slo:postalAddress      \
                                                       [ nco:locality ?cty ;  \
                                                         nco:country  ?cry ]  \
                                                     ] .                      \
                                                    }'
Results:
  file:///home/user/MyDocs/DCIM/20110726_001.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_002.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_003.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_004.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_005.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_006.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_007.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_008.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_009.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_010.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_011.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_012.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_013.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_014.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_015.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_016.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_017.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_018.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_019.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_020.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_021.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_022.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_023.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_024.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_025.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_026.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_027.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110726_028.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110730_001.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110730_002.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110730_003.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110731_002.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110731_003.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110807_001.mp4, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110807_002.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110807_003.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110813_001.mp4, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110814_001.mp4, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110815_001.mp4, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110815_002.mp4, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110815_003.mp4, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110822_002.mp4, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110824_013.mp4, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110908_001.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110908_002.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110908_003.mp4, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110908_004.mp4, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110909_001.mp4, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110910_001.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110911_001.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110911_002.mp4, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110912_001.mp4, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110912_002.mp4, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110912_003.mp4, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20110912_004.mp4, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20111012_002.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20111012_003.mp4, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20111017_001.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20111017_002.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20111017_003.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20111017_004.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20111017_005.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20111017_006.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20111113_007.jpg, Corona Del Mar, UNITED STATES
  file:///home/user/MyDocs/DCIM/20111014_001.jpg, Newport Beach, UNITED STATES
  file:///home/user/MyDocs/DCIM/20111014_002.jpg, Newport Beach, UNITED STATES
```