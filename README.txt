TG3149 DMR Utah Facebook Group
Anytone Code Plug

Welcome! See Docs/INSTALL.txt for installation instructions. Before modifying any talkgroups or channels, read Docs/Editing.txt for helpful tips.

Need help? Contact:
N2OW, Ryan Simpkins
simpkins.ryan@gmail.com
801-602-8661
DMR ID: 3177246 (I accept private calls)

See a demo of this Code Plug here: https://youtu.be/SQrn46a8I_s

CHANGE LOG:
===v1.3===
See a demo of v1.3 here: https://youtu.be/tIrOZ-0PQLM

* Added 591 new analog channels & 5 analog zones including:
*** All UTVHFS simplex frequencies (VHF & UHF).
*** All UTVHFS listed repeaters (VHF & UHF).
*** SLCo ARES Standard Load (March 2021).
* Fully implemented Analog APRS for analog zones.
*** Update callsign in APRS options before use.
*** Analog APRS is disabled in the SLCo ARES zone.
* Change digital APRS repeater delay from 100ms to 200ms to improve reliability.
* Added version number in boot display
* Added disconnect TG for TGIF DMR GW config (4004000).
* Included Anytone CPS DCF file, see Data/ directory.
* Some scan lists added. See "KNOWN ISSUES" below.
* Updated several docs, images, and data files.

===v1.2===
* Fixed major TG sorting error introduced by Anytone CPS bug.
* Included data exports in Data/ directory to help work around bugs.
* Included fixes for analog APRS (untested at this stage).
* Added additional documentation.
* Added note regarding radio modes from W0AKO. See Docs/Change Mode.
* TG list slightly reordered... again... because bugs.

===v1.1===
* TGIF TG for Utah added (4003149).
* TG list slightly reordered.
* Documentation added (see Docs folder).
* Screenshots of optional settings added. (CPS doesn't support exporting these!)

===v1.0===
* Functional Digital APRS. Simply enable GPS.
* More hotspots, including Utah VHF Society recommended hotspot frequency: 438.525Mhz as default.
* Support for Duplex hotspots. UPDATE FREQUENCIES BEFORE USE!
* Removes redundant timeslot channels. Use a quick key to switch timeslots.
* Updated TG list current as of 25 March, 2021.
* Tons of additional TGs added in the contact/TG list, all organized by category! Each category begins with an underscore (e.g. _UTAH TGs).
* Experimental support for Western States repeaters in St. George and Las Vegas.
* Support for TGIF network. See Docs/TGIF.txt for info.
* Support for pi-star remote. See Docs/PISTAR_REMOTE.txt for info.
* Disconnect & parrot mapped to every zone.
* Several more default channels for popular TGs added.
* Consistent channel names between all zones.
* Room in the file to easily add additional channels and TGs.
* SMS quick text populated with standard messages.
* All optional settings updated for easy operation.
* Support for OpenSpot telemetry from Simplex hotspots (thanks to KI7GGG for assist!).
* Talker alias display support.
* Open "shim" zone to make manually adding an ad-hoc repeater possible from the radio's menu system (no software needed).


KNOWN ISSUES:

=Talkgroup Spacing=
* Sometimes the TG list spacing gets messed up in the CPS software. If this happens:
1) Re-import the TG list from the Data/Talkgroups.csv file.
2) Save.
3) Re-import channels from the Data/Channels.csv file.
4) Save.

=Radio Mode (Out of Band error)=
* Requires the radio be in Amatuer Mode (000007). If you have an older radio this might need to be fixed, which isn't simple at all. Contact me if it doesn't work. You can check the mode by using the CPS drop down menu Model->Model Information while the radio is connected to CPS. Note that this only impacts tx ranges. You can still rx over the full Anytone range.

=Selecting Channels=
* The analog zones have many channels. It appears that a bug in the Anytone firmware will not allow a user to quickly select channels above 159 using the keypad. You can enter "159" for example, but not "160." The channel selection wheel at the top of the radio will allow you to select channels above 159. If we discover a workaround, we will update this document.

=Scan List Limitations=
* Anytone does not support more than 50 channels in a scan list. This significantly limits the usefulness of scan lists for analog frequencies and systems. The current code plug has over 590 analog channels. It would take 12 unique scan lists to cover everything, and could only be scanned one bank at a time. For now, operators can build their own scan lists if they wish. Until this capability is improved by Anytone, we will not be adding any additional scan lists.

=Parrot on TGIF=
Parrot isn't working when using the TGIF DMR Gateway feature. We are looking in to it. No update at this time.