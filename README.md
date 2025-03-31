# note2q
Max 4 live device that translates Midi Notes to MSC meant to trigger light cues.

--
Takes Note ON and triggers MSC through Sysex. 

The specific MSC command is "Device ID - General Lighting - GO cue 'midi note'", as described on
https://help2.malighting.com/Page/grandMA2/remote_control_msc/en/3.9.

Meant to work with the selected cuelist on GrandMA 2 consoles.

Current limitations: cue on MA needs to be a whole number between 1 and 127, and one cannot trigger cues in multiple cue lists.
Filters incoming midi by "note on", ignores velocity.
