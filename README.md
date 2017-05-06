# Dr.Drums
This is an advanced system for generating electronic dance music (EDM) drum loops based on the concept of *style*. The system has embeded statistical knowledge on how drum patterns in different EDM styles are programmed, making this software very useful for generating new coherent and stylysh drum patterns automatically. I see this software as a tool to amplify the creativity of beat makers helping them get a really fast kickstart and as a straightforward tool for exploring how a drum pattern composed of different styles can be realized. As the system is based on statistical data, there are no fixed or preset patterns, a style is now a seen as a region in a highly dimensional space and a pattern as a vector in that space, so virtualy endless pattern possibilities can be generated. As an enhancement for real-time generation and amnipulation of drumming, I have introduced some elastic editing tools that allow each instrument's pattern (i.e the pattern of the claps or the rimshot) to be dramatically transformed by increasing or decreasing its density (density = the amount of onsets) but with a reversible effect so that found sweet spots can always be recovered.

The main features:
* There is drumming knowledge on House, Techno, Breakbeat, Garage, Soul and Hip-Hop styles.
* Two styles can be mixed using a crossfade slider. In this way, one can go, for example, from straight House style loops to straight Breakbeat loops continously. Finding a "pure" style at each end of the slider and new "hybrid" styles allover the slider range.
* Up to demo 10.1 drum loops are composed of 32 step (2 bar) patterns. From demo 10.2 on loops are limited to 16 step (1 bar) loops. Using demo 10.2 is recomended.
* So far, the patterns are limited to 8 instruments: kick, snare, closed hi-hat, open hi-hat, clap, rimshot, low conga and hi conga.
* Each instrument has a smart "Density" slider which adds or subtracts onsets, allowing real time editing of the pattern in a continous fashion. This slider adds or subtracts onsets without distorting the main characteristics of the pattern, respecting main syncopations and reinforcements that make the character of the pattern.
* A "new" button can be clicked ad-infinitum to generate new patterns based on the two styles selected and the position of the Crossfade slider. For example, if the styles selected are Techno and Garage and the slider is right in its middle (50% Techno 50% Garage)a new Techno-Garage pattern will emerge every time the "New" button is pressed.
* Each instrument can be muted. 
* Each instrument can also be transformation-disabled so that dynamic transformations only affect certain instruments of the pattern.
* Presets can be saved, saving the pattern and the settings of all parameters for further sessions.

In each .zip file there are two puredata (pd) patches. One patch called Wstand alone" lets you generate patterns and listen to them when opening it in pd. The other pd patch called "DAW" does not reproduce audio but syncs to MIDI clock tempo and sends MIDI note on messages for every instrument that is to be played. Therefore if you want to integrate this software with your virtual or analog beat station you only need to send a local MIDI time clock message to pd.

#Instructions for standalne use
1. Download and install Puredata 'vanilla' from http://puredata.info/downloads.
2. Download Demo_10.2.zip from this link: https://github.com/danielgomezmarin/mididrums/raw/master/demo10.2.zip.
3. Uncompress the zip file.
4. Open DrDrumsV10.2_Standalone.pd

#Important Notes
If you have come here its most likely beacuse I have invited you. As this is an experimental software produced as a proof of concept during my PhD thesis, I would love to hear from you and get some feedback on some specific aspects of this software. It would be great if you could take your time and send me an email with your comments regarding the conceptual aspects that have been consudered for its conception. Some useful questions could be: how do you find the patterns created? do tehy fulfill your stylystic conceptions? Do you find it useful for production, for real time interaction or for both? Would you use it on a day to day basis? Would you like to add a specific feature?

Very imoprtantly, keep in mind that the style knowledge is based on real life examples and it can be expanded on demand. This inevitably leads to the possibility of loading this software with *YOUR* style. Or with the style of your previous record. Or to create knowledge on any other drumming style ouside EDM that suits you. So, if you are interested in customizing this software so that it knows a specific style which you have at hand (preferably as MIDI files from your DAW) get in touch.
