This is a JS percussion SoundFont that is compatible with [MIDI.js](https://github.com/mudcube/MIDI.js) and [soundfont-player](https://github.com/danigb/soundfont-player).

##Usage
The drum names are listed in [drums.json][https://github.com/notochord/percussion-soundfont.js/blob/master/drums.json].

###With MIDI.js
Note that MIDI.js can only handle one SoundFont at a time, so you're stuck either using drums or other instruments.
```javascript
MIDI.soundfontUrl = 'https://notochord.github.io/percussion-soundfont.js/';
MIDI.loadPlugin({
    instrument: "percussion",
    onsuccess: function() { }
});
```


With soundfont-player:

```javascript
Soundfont.instrument(ac, 'percussion-mp3.js', { from: 'https://notochord.github.io/percussion-soundfont.js/' })
```

##Credits
This is an adaptation of the [GeneralUser](http://www.schristiancollins.com/generaluser.php) SoundFont, and was converted to JS by [https://github.com/letoribo] in [this repository](https://github.com/letoribo/General-MIDI-Percussion-soundfonts-for-MIDI.js-).
I just put the files in this repo for safekeeping, but [https://github.com/letoribo] gets all the credit for the actual conversion.
Check out their project [drums.herokuapp.com](https://drums.herokuapp.com/)!
