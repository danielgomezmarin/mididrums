# mididrums
Expert system for generating MIDI loops in electronic dance music (EDM) styles coded in PureData. The system has statistical knowledge on how drum patterns in different EDM styles are programmed allowing to generate new rhythmic material very easily. I see this software as a tool to amplify the creativity of EDM beat makers by helping them get a really fast kickstart and very easily try style mixtures with the twist of a knob. As the system is based on statistical data, there are no fixed or preset patterns, a style is a seen as a region in a highly dimensional space and a pattern a vector in that space, so virtualy endless pattern possibilities can be generated. There are some real-time elastic editing tools allowing a drum pattern to be dramatically transformed but with a reversible effect so it can always be recovered.

features as:
* There is drumming knowledge on House, Techno, Breakbeat, Garage, Soul and Hip-Hop.
* Two styles can be mixed using a crossfade slider. In this way, one can go, for example, from straight House style loops to straight Breakbeat loops continously. Finding a "pure" style at each end of the slider and new "hybrid" styles allover the slider range.
* Up to demo 10.1 drum loops are composed of 32 step (2 bar) patterns. From demo 10.2 on loops are limited to 16 step (1 bar) loops.
* The patterns are limited to 8 instruments: kick, snare, closed hi-hat, open hi-hat, clap, rimshot, low conga and hi conga.
* Each instrument has a "Density" slider which adds or subtracts onsets, allowing real time editing of the pattern in a continous fashion.
* A "new" button can be clicked ad-infinitum to generate a new pattern based on the two styles selectd and the position of the Crossfade slider. For example, if the styles selected are Techno and Garage and the slider is right in its middle (50% Techno 50% Garage)a new Techno-Garage pattern will emerge every time the "New" button is pressed.
* Each instrument can be muted. 
* Each instrument can also be transformation-disabled so that dynamic transformations only affect certain instruments of the pattern.
* Presets can be saved, saving the pattern and the settings of all parameters.

There are two patches in each .zip file. One which lets you generate patterns and listen to them using puredata which is called the stand Alone" version. An the other that does not reproduce audio but that syncs to MIDI clock tempo and sends MIDI note on messages for every instrument that is to be played.

The .zip files contain everything necesary to run the demos. You only need to download puredata "vanmilla" from http://puredata.info/downloads.
