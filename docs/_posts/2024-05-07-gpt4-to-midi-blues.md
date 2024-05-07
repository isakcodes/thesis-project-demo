---
layout: post
title:  "Experiment: GPT-4 to MIDI [Blues]"
date:   2024-05-07 19:05:00 +0200
categories: gpt
---

**Role: system**

```
You are MusicGPT, a music creation and completion chat bot that.
When a user gives you a prompt, you return them a song showing 
the notes, durations, and times that they occur. Respond with just the music.

Notation looks like this:
(Note-duration-time in beats)
C4-1/4-0, Eb4-1/8-2.5, D4-1/4-3, F4-1/4-3 etc.
```


<h1>Prompt, Response and MIDI</h1>
<div id="listening-area-1" class="listening-area">
  <div class="tab"></div>
  <div id="player">
    <p class="helptext">Select one of the tabs, then press play to listen.</p>
    <midi-visualizer type="piano-roll" id="mainVisualizer" src=""></midi-visualizer>
    <midi-player src="" sound-font visualizer="#mainVisualizer" id="mainPlayer"></midi-player>
  </div>
  <div id="files-list-area" hidden="True">
    <h2>Files</h2>
    <ul class="midifiles">
      <li><a class="afile" href="https://raw.githubusercontent.com/isakcodes/GPT-4-To-MIDI/993ba68a0ef40b6342f3ba723360ec5f108b2003/out/blues/combined0.mid" displayName="0">0</a></li>
      <li><a class="afile" href="https://raw.githubusercontent.com/isakcodes/GPT-4-To-MIDI/993ba68a0ef40b6342f3ba723360ec5f108b2003/out/blues/combined1.mid" displayName="1">1</a></li>
      <li><a class="afile" href="https://raw.githubusercontent.com/isakcodes/GPT-4-To-MIDI/993ba68a0ef40b6342f3ba723360ec5f108b2003/out/blues/combined2.mid" displayName="2">2</a></li>
      <li><a class="afile" href="https://raw.githubusercontent.com/isakcodes/GPT-4-To-MIDI/993ba68a0ef40b6342f3ba723360ec5f108b2003/out/blues/combined3.mid" displayName="3">3</a></li>
    </ul>
  </div>
</div>

**User:**

<div markdown="1" class="text-note" hidden="True" displayName="0">

`A suitable melody for the chord progression in this midi file please`
(*...followed by the midi file converted to note-duration-time format.*)

</div>
<div markdown="1" class="text-note" hidden="True" displayName="1">

`Could you please make it a bit more interesting? While sticking to the timing given by the chord progression.`

</div>
<div markdown="1" class="text-note" hidden="True" displayName="2">

`The genre for the Chord Progression is Blues. Can you make something that is more typical for the Blues genre? Without being too boring.`

</div>
<div markdown="1" class="text-note" hidden="True" displayName="3">

`Now, please do your best to produce a melody which a musician, when hearing together with the chord progression, would believe was made by a human.^[[D` (sic)

</div>



**GPT-4:**

<div markdown="1" class="text-note" hidden="True" displayName="0">

```
Sure, here's a melody over your chord progression:

Eb5-1/4-0, F5-1/8-1, Eb5-1/8-1.5, D5-1/2-2, Eb5-1/2-3, C5-1/8-5, Bb4-1/8-5.5, Ab4-1/8-6, G4-1/8-6.5, F4-1/4-7, G4-1/4-8, Ab4-1/4-9, Bb4-1/4-10, C5-1/2-11, Bb4-1/4-13, Ab4-1/4-14, G4-1/2-15, F4-1/2-16, Eb4-1/2-17, C4-1/4-18, Eb4-1/8-18.5, F4-1/4-19, G4-1/2-20, Ab4-1/2-21, Bb4-1/4-22, C5-1/4-23, D5-1/2-24, Eb5-1/4-26, F5-1/8-27, Eb5-1/8-27.5, D5-1/4-28, Ab4-1/4-29, F4-1/2-30, G4-1/2-31.
```

</div>
<div markdown="1" class="text-note" hidden="True" displayName="1">

```
Certainly! Here is a more expansive melody:

Eb5-1/4-0, F5-1/16-0.75, Eb5-1/16-1, D5-1/8-1.25, Ab4-1/4-2, Bb4-1/8-3, Ab4-1/8-3.5, G4-1/8-4, F4-1/16-4.75, Bb4-1/8-5, Ab4-1/4-5.5, G4-1/8-6, F4-1/8-6.5, G4-1/4-7, C5-1/2-7.75, F5-1/8-8, G4-1/4-8.5, Ab4-1/4-9, G4-1/4-9.5, F4-1/8-10, G4-1/4-10.5, Eb4-1/8-11, D4-1/4-12, Eb4-1/4-12.5, F4-1/8-13, G4-1/4-13.5, Ab4-1/4-14, Bb4-1/4-15, C5-1/2-15.5, Eb5-1/2-16, D5-1/4-17, Eb4-1/8-17.5, F4-1/8-18, G4-1/4-18.5, Ab4-1/8-19, Bb4-1/4-19.5, C5-1/4-20, D5-1/2-22, Eb5-1/4-22.5, F5-1/8-23, G5-1/2-23.5, F5-1/2-24, Eb5-1/4-25, D5-1/4-26, Bb4-1/8-27, Ab4-1/8-27.5, G4-1/4-28, F4-1/8-28.5, G4-1/2-29, Bb4-1/4-30, C5-1/4-31.

This melody features more intricate rhythms and some faster note changes to create a stronger sense of movement and interest.
```

</div>
<div markdown="1" class="text-note" hidden="True" displayName="2">

```
Certainly! Blues melodies often feature repeated motifs, blue notes, and a more laid-back, syncopated rhythm. Let's try this:

Eb5-1/4-0, D5-1/8-1, Eb5-1/8-1.5, D5-1/4-2, C5-1/4-2.5, Bb4-1/8-3, Ab4-3/8-3.5, Bb4-1/8-4, F4-1/4-4.5, Bb4-3/4-5, Ab4-1/4-6, Bb4-1/8-6.5, Eb5-1/8-7, D5-1/4-7.5, Eb5-1/4-8, D5-1/4-8.5, C5-1/8-9, Bb4-1/4-9.5, C5-1/8-10, D5-1/8-10.5, Eb5-1/4-11, D5-1/8-11.5, C5-1/8-12, Bb4-1/8-12.5, C5-1/8-13, Bb4-1/4-13.5, Ab4-1/4-14, Bb4-1/8-14.5, C5-1/8-15, D5-1/4-15.5, Eb5-1/4-16, D5-1/8-16.5, C5-1/8-17, Bb4-1/8-17.5, Ab4-1/8-18, Bb4-1/8-18.5, F4-1/2-19, Eb4-1/2-20, D5-1/4-21, Eb5-1/4-22, F5-1/4-23, G5-1/4-24, F5-1/8-24.5, Eb5-1/8-25, D5-1/4-25.5, C5-1/2-26, Ab4-1/2-27, Bb4-1/4-28, Ab4-1/8-28.5, G4-1/8-29, F4-1/2-30, Bb4-1/4-31, C5-1/4-32.

This should evoke more of a blues feeling while still maintaining interest and complexity.
```

</div>
<div markdown="1" class="text-note" hidden="True" displayName="3">

```
Sure, here's a bluesy melodic line keeping it catchy and memorable:

Eb5-1/2-0, Ab4-1/2-1, Bb4-1/4-2, Ab4-1/4-2.5, G4-1/4-3, F4-1/4-3.5, Ab4-1/4-4, Bb4-1/4-4.5, C5-1/2-5, Bb4-1/4-7, Ab4-3/8-7.5, G4-1/2-8, F4-1/4-9, Eb4-1/2-9.5, F4-3/8-11, G4-3/8-12, Ab4-1/4-14, Bb4-1/8-14.5, C5-1/4-15, D5-1/4-15.5, Eb5-1/8-16, C5-1/8-16.5, Bb4-1/2-17, Ab4-1/4-18.5, G4-1/4-19.5, F4-1/2-20, G4-1/4-21, Ab4-1/4-22, Bb4-1/2-23, C5-1/2-24, D5-1/2-25, Eb5-1/4-26, C5-1/8-26.5, Bb4-1/8-27, Ab4-1/4-27.5, G4-3/8-28, F4-1/2-29, Eb4-3/8-30, F4-1/8-31, G4-1/8-31.5, Ab4-1/4-32.

This should evoke a bluesy and melodic feeling that should match perfectly with the chord progression provided.
```

</div>
<br>

---

## Files etc

**Source code:** [g2m.py](https://raw.githubusercontent.com/isakcodes/GPT-4-To-MIDI/993ba68a0ef40b6342f3ba723360ec5f108b2003/g2m.py)

**Attribution:** Fork of [original work by d3n7 on GitHub](https://github.com/d3n7/GPT-4-To-MIDI) with small modifications.


<details markdown="1"><summary>Files</summary>

- All output files [out/blues/](https://github.com/isakcodes/GPT-4-To-MIDI/tree/7da2bee8d5d7d6a104eeb4827b712e2dd8e3314a/out/blues)
- [Terminal log file](https://raw.githubusercontent.com/isakcodes/GPT-4-To-MIDI/my_experiments/out/blues/log.txt)

</details>


{% raw %}
<script>
window.addEventListener('DOMContentLoaded', () => {
  var afiles = document.querySelectorAll('#files-list-area > ul > li > a');
  var tab = document.querySelector('.listening-area > .tab');
  var filesListArea = document.querySelector('#files-list-area');
  afiles.forEach((afile) => {
    var button = document.createElement('button');
    button.className = 'tablinks';
    button.textContent = afile.getAttribute('displayName');
    button.onclick = function(event) {
      openTab(event, afile.href);
    };
    tab.appendChild(button);
  });
});

function openTab(event, midiFile) {
  var i, tablinks;
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  event.currentTarget.className += " active";

  var midiVisualizer = document.getElementById('mainVisualizer');
  var midiPlayer = document.getElementById('mainPlayer');
  
  midiVisualizer.src = midiFile;
  midiPlayer.src = midiFile;

  var tabInstruction = event.currentTarget.parentElement.parentElement.querySelector('.helptext');
  if (tabInstruction) {
    tabInstruction.remove();
  }

  var allNotes = document.getElementsByClassName('text-note');
  for (i = 0; i < allNotes.length; i++) {
      allNotes[i].setAttribute('hidden', true);
  }

  var selectionTextContent = event.target.textContent;
  var correspondingTextNoteDivs = document.querySelectorAll('div[displayName="'+selectionTextContent+'"]');

  for (i = 0; i < correspondingTextNoteDivs.length; i++) {
    if (correspondingTextNoteDivs.displayText == event.currentTarget.displayText) {
      correspondingTextNoteDivs[i].removeAttribute('hidden');
    }
  }
}
</script>
{% endraw %}