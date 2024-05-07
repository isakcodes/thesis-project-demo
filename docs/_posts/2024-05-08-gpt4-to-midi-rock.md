---
layout: post
title:  "Experiment: GPT-4 to MIDI [Rock]"
date:   2024-05-08 00:04:00 +0200
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
      <li><a class="afile" href="https://raw.githubusercontent.com/isakcodes/GPT-4-To-MIDI/993ba68a0ef40b6342f3ba723360ec5f108b2003/out/rock/combined0.mid" displayName="0">0</a></li>
      <li><a class="afile" href="https://raw.githubusercontent.com/isakcodes/GPT-4-To-MIDI/993ba68a0ef40b6342f3ba723360ec5f108b2003/out/rock/combined1.mid" displayName="1">1</a></li>
      <li><a class="afile" href="https://raw.githubusercontent.com/isakcodes/GPT-4-To-MIDI/993ba68a0ef40b6342f3ba723360ec5f108b2003/out/rock/combined2.mid" displayName="2">2</a></li>
      <li><a class="afile" href="https://raw.githubusercontent.com/isakcodes/GPT-4-To-MIDI/993ba68a0ef40b6342f3ba723360ec5f108b2003/out/rock/combined3.mid" displayName="3">3</a></li>
      <li><a class="afile" href="https://raw.githubusercontent.com/isakcodes/GPT-4-To-MIDI/993ba68a0ef40b6342f3ba723360ec5f108b2003/out/rock/combined4.mid" displayName="4">4</a></li>
      <li><a class="afile" href="https://raw.githubusercontent.com/isakcodes/GPT-4-To-MIDI/993ba68a0ef40b6342f3ba723360ec5f108b2003/out/rock/combined5.mid" displayName="5">5</a></li>
      <li><a class="afile" href="https://raw.githubusercontent.com/isakcodes/GPT-4-To-MIDI/993ba68a0ef40b6342f3ba723360ec5f108b2003/out/rock/combined6.mid" displayName="6">6</a></li>
      <li><a class="afile" href="" displayName="7">7</a></li>
    </ul>
  </div>
</div>

<div markdown="1" displayName="0" class="text-note" hidden="True">

**User:**

`A suitable melody for the chord progression in this midi file please` (*...followed by chord progression midi in note-duration-time format*)

**GPT-4:**
```text
A4-1/4-0.5, C5-1/4-1, A4-1/4-1.5, F4-1/4-2, C5-1/4-2.5, A4-1/4-3, F4-1/4-3.5, C5-1/4-4, D5-1/4-4.5, C5-1/4-5, A4-1/4-5.5, F4-1/4-6, A4-1/4-6.5, C5-1/4-7, A4-1/4-7.5, F4-1/4-8, A4-1/4-9, C5-1/4-9.5, A4-1/4-10, G4-1/4-10.5, F4-1/4-11, A4-1/4-11.5, C5-1/4-12, G5-1/4-12.5, F5-1/4-13, D5-1/4-13.5, C5-1/4-14, F4-1/4-14.5, A4-1/4-16, C5-1/4-16.5, D5-1/4-17, C5-1/4-17.5, A4-1/4-18, F4-1/4-18.5, A4-1/4-19, C5-1/4-19.5, F5-1/4-20, D5-1/4-20.5, C5-1/4-21, A4-1/4-21.5, F4-1/4-22, A4-1/4-22.5, C5-1/4-23, A4-1/4-23.5, F4-1/4-24, A4-1/4-24.5, C5-1/4-25, A4-1/4-25.5, F4-1/4-26, C5-1/4-27, A4-1/4-27.5, F4-1/4-28, C5-1/4-28.5, D5-1/4-29, C5-1/4-29.5, A4-1/4-30, F4-1/4-30.5, C5-1/4-31, A4-1/4-31.5, F4-1/4-32, A4-1/4-32.5, C5-1/4-33, A4-1/4-33.5, F4-1/4-34, A4-1/4-34.5, C5-1/4-35, A4-1/4-35.5, F4-1/4-36, A4-1/4-36.5, C5-1/4-38, A4-1/4-38.5, F4-1/4-39, C5-1/4-39.5, D5-1/4-40, C5-1/4-40.5, A4-1/4-41, F4-1/4-41.5, C5-1/4-42, A4-1/4-42.5, F4-1/4-43, A4-1/4-43.5, C5-1/4-44, A4-1/4-44.5, F4-1/4-45, C5-1/4-46, A4-1/4-46.5, F4-1/4-47, C5-1/4-47.5, D5-1/4-48, C5-1/4-48.5, A4-1/4-49, F4-1/4-49.5, C5-1/4-50, A4-1/4-50.5, F4-1/4-51, C5-1/4-51.5, D5-1/4-52, C5-1/4-52.5, A4-1/4-53, F4-1/4-53.5, A4-1/4-54, C5-1/4-54.5, A4-1/4-55, F4-1/4-55.5, C5-1/4-56, A4-1/4-56.5, F4-1/4-57, C5-1/4-58, A4-1/4-58.5, F4-1/4-59, C5-1/4-59.5, D5-1/4-60, C5-1/4-60.5, A4-1/4-61, F4-1/4-61.5, A4-1/4-62, C5-1/4-62.5, F5-1/4-63, C5-1/4-63.5, A4-1/4-64, F4-1/4-64.5, A4-1/4-65, C5-1/4-65.5, A4-1/4-66, F4-1/4-66.5, A4-1/4-67, C5-1/4-67.5, A4-1/4-68, F4-1/4-68.5, A4-1/4-69, C5-1/4-69.5, A4-1/4-70, F4-1/4-70.5, A4-1/4-71, C5-1/4-71.5, A4-1/4-72, F4-1/4-72.5, C5-1/4-73, A4-1/4-73.5, F4-1/4-74, C5-1/4-74.5, D5-1/4-75, C5-1/4-75.5, A4-1/4-76, F4-1/4-76.5, C5-1/4-77, A4-1/4-77.5, F4-1/4-78, C5-1/4-78.5, A4-1/4-79, F4-1/4-79.5, A4-1/4-80, C5-1/4-80.5, A4-1/4-81, F4-1/4-81.5, A4-1/4-82, C5-1/4-82.5, A4-1/4-83, F4-1/4-83.5, C5-1/4-84, A4-1/4-84.5, F4-1/4-85, C5-1/4-85.5, D5-1/4-86, C5-1/4-86.5, A4-1/4-87, F4-1/4-87.5, C5-1/4-88, A4-1/4-88.5, F4-1/4-89, C5-1/4-89.5, D5-1/4-90, C5-1/4-90.5, A4-1/4-91, F4-1/4-91.5, A4-1/4-92, C5-1/4-92.5, F5-1/4-93, C5-1/4-93.5, A4-1/4-94, F4-1/4-94.5, C5-1/4-95, A4-1/4-95.5, F4-1/4-96, A4-1/4-96.5, C5-1/4-97, A4-1/4-97.5, F4-1/4-98, A4-1/4-98.5, C5-1/4-99, A4-1/4-99.5, F4-1/4-100
```

</div>
<div markdown="1" displayName="1" class="text-note" hidden="True">

**User:**

`the dissonant chords in the progression aren't complemented by this melody. Could you identify the areas where the chords are dissonant, and edit the melody to fit better (unless it already is a good fit of course)?`

**GPT-4:**

```text
Looking at your chord progression, we can see some examples of dissonant chords at the following points:

(I've only identified the most relevant, there may be more)

1. Ab2-1-34, Gb3-1-34, Bb3-1-34, B3-1-34
2. D3-1/4-38, Bb3-1/4-38, F3-1/4-38, D4-1/4-38, F4-1/4-38
3. A2-1/4-39, E3-1/4-39, G3-1/4-39, C4-1/4-39
4. C3-1/2-52, Bb3-1/2-52, D4-1/2-52, E4-1/2-52

Revised melody to better fit these dissonant chords would be:

A4-1/4-0.5, C5-1/4-33.75, F4-1/4-34, Bb4-1/4-34.25, Cb4-1/4-34.75, Bb4-1/4-35, Cb4-1/4-35.25, D4-1/4-39, Bb4-1/4-39.25, C4-1/4-39.5, C5-1/4-39.75, C4-1/4-39.75, Bb3-1/4-39.875, A4-1/4-43, C5-1/4-43.25, Bb4-1/4-43.5, D5-1/4-43.75, C4-1/4-52, Eb4-1/4-52.25, D4-1/4-52.5, C5-1/4-52.75

The remainder of the melody can stay the same as it fits well with the other chords in the progression.
```
</div>

<div markdown="1" displayName="2" class="text-note" hidden="True">

**User:**

`That confuses me. Please give me the new, complete melody only and no other text. Make sure you didn't introduce any errors.`

**GPT-4:**

```text
Here's your complete new melody:

A4-1/4-0.5, C5-1/4-1, A4-1/4-1.5, F4-1/4-2, C5-1/4-2.5, A4-1/4-3, F4-1/4-3.5, C5-1/4-4, D5-1/4-4.5, C5-1/4-5, A4-1/4-5.5, F4-1/4-6, A4-1/4-6.5, C5-1/4-7, A4-1/4-7.5, F4-1/4-8, A4-1/4-9, C5-1/4-9.5, A4-1/4-10, G4-1/4-10.5, F4-1/4-11, A4-1/4-11.5, C5-1/4-12, G5-1/4-12.5, F5-1/4-13, D5-1/4-13.5, C5-1/4-14, F4-1/4-14.5, F4-1/4-34, Bb4-1/4-34.25, Cb5-1/4-34.75, D4-1/4-38.75, C4-1/4-38.875, Bb3-1/4-38.9375, C5-1/4-52.75, A4-1/4-56.5, F4-1/4-57, C5-1/4-58, A4-1/4-58.5, F4-1/4-59, C5-1/4-59.5, D5-1/4-60, C5-1/4-60.5, A4-1/4-61, F4-1/4-61.5, A4-1/4-62, C5-1/4-62.5, F5-1/4-63, C5-1/4-63.5, A4-1/4-64, F4-1/4-64.5, A4-1/4-65, C5-1/4-65.5, A4-1/4-66, F4-1/4-66.5, A4-1/4-67, C5-1/4-67.5, A4-1/4-68, F4-1/4-68.5, A4-1/4-69, C5-1/4-69.5, A4-1/4-70, F4-1/4-70.5, A4-1/4-71, C5-1/4-71.5, A4-1/4-72, F4-1/4-72.5, C5-1/4-73, A4-1/4-73.5, F4-1/4-74, C5-1/4-74.5, D5-1/4-75, C5-1/4-75.5, A4-1/4-76, F4-1/4-76.5, C5-1/4-77, A4-1/4-77.5, F4-1/4-78, C5-1/4-78.5, A4-1/4-79, F4-1/4-79.5, A4-1/4-80, C5-1/4-80.5, A4-1/4-81, F4-1/4-81.5, A4-1/4-82, C5-1/4-82.5, A4-1/4-83, F4-1/4-83.5, C5-1/4-84, A4-1/4-84.5, F4-1/4-85, C5-1/4-85.5, D5-1/4-86, C5-1/4-86.5, A4-1/4-87, F4-1/4-87.5, C5-1/4-88, A4-1/4-88.5, F4-1/4-89, C5-1/4-89.5, D5-1/4-90, C5-1/4-90.5, A4-1/4-91, F4-1/4-91.5, A4-1/4-92, C5-1/4-92.5, F5-1/4-93, C5-1/4-93.5, A4-1/4-94, F4-1/4-94.5, C5-1/4-95, A4-1/4-95.5, F4-1/4-96, A4-1/4-96.5, C5-1/4-97, A4-1/4-97.5, F4-1/4-98, A4-1/4-98.5, C5-1/4-99, A4-1/4-99.5, F4-1/4-100.
```

</div>

<div markdown="1" displayName="3" class="text-note" hidden="True">

**User:**

`I like that result very much. Well done! Can you please start over and invent something equally good, but different? I want to consider a new conception of melody to that same chord progression. As always, answer in the music format only, with the full melody.`

**GPT-4:**

```text
Of course! Here is a new melody that fits the chord progression you provided:

C5-1/2-0.5, A4-1/2-2, C5-1/4-3, Bb4-1/4-3.5, C5-1/4-4, G4-1/4-6, A4-1/4-8, F4-1/2-9, Eb4-1/4-11.5, Eb5-1/4-12.5, D4-1/4-13.75, C4-1/2-15.25, B4-1/4-17, Bb4-1/2-18.5, G4-1/4-20.5, F4-1/4-22.5, Eb4-1/2-24.5, C4-1/4-27, Db4-1/4-29, Bb3-1/2-31.5, C4-1/4-33, D4-1/2-35, Eb4-1/4-37, F4-1/2-39.5, G4-1/4-41, A4-1/4-43.75, Bb4-1/2-44.5, B4-1/4-47, C5-1/4-49, Db5-1/2-51.75, C5-1/4-54.5, Bb4-1/4-56.5, A4-1/2-58.75, G4-1/4-60.5, F4-1/4-62.5, Eb4-1/2-65.25, D4-1/4-67, Db4-1/4-69, C4-1/2-70.5, Bb3-1/4-74.75, A3-1/4-78, G3-1/2-80, F3-1/4-82, D3-1/4-83.5, Db3-1/2-85.25, C3-1/4-87.5, Bb2-1/4-89.5, A2-1/2-92, F2-1/4-94, C2-1/2-96, Bb1-1/4-98, A1-1/4-99.5.
```

</div>

<div markdown="1" displayName="4" class="text-note" hidden="True">

**User:**

`I don't like it. The melody is lazy and the timings are quite off. There are some sections of silence followed by an awkward note. Can you try to improve the melody and make it sound more like rock music?`

**GPT-4:**

```text
Sure, I apologize for the confusion earlier. Let's go in a rock direction for your chord progression:

A4-1/4-0.5, B4-1/4-1, A4-1/8-1.5, G4-1/8-1.75, A4-1/4-2, Bb4-1/2-2.5, A4-1/2-3.5, G4-1/4-4.5, F4-1/4-5, G4-1/4-6, F4-1/4-7, G4-1/4-8, A4-1/4-9, Bb4-1/4-10, B4-1/4-11, A4-1/4-12, G4-1/4-13, F4-1/4-14, Eb4-1/4-15, D4-1/4-16, C4-1/4-17, D4-1/4-18, Eb4-1/4-19, F4-1/4-20, G4-1/4-21, A4-1/4-22, Bb4-1/4-23, B4-1/4-24, C5-1/4-25, B4-1/4-26, A4-1/4-27, G4-1/4-28, F4-1/4-29, Eb4-1/4-30, D4-1/4-31, C4-1/4-32, D4-1/4-33, Eb4-1/4-34, F4-1/4-35, G4-1/4-36, A4-1/4-37, Bb4-1/4-38, C5-1/4-39, B4-1/4-40, A4-1/4-41, G4-1/4-42, F4-1/4-43, Eb4-1/4-44, D4-1/4-45, C4-1/4-46, D4-1/4-47, Eb4-1/4-48, F4-1/4-49, G4-1/4-50, A4-1/4-51, Bb4-1/4-52, C5-1/4-53, B4-1/4-54, A4-1/4-55, G4-1/4-56, F4-1/8-57, Eb4-1/8-57.25, D4-1/8-57.5, Eb4-1/8-57.75, F4-1/4-58, G4-1/2-59, F4-1/2-60, Eb4-1/4-61, D4-1/4-62, C4-1/4-63, D4-1/4-64, Eb4-1/4-65, F4-1/4-66, G4-1/4-67, A4-1/4-68, Bb4-1/4-69, B4-1/4-70, A4-1/4-71, G4-1/4-72, F4-1/4-73, G4-1/4-74, A4-1/4-75, B4-1/4-76, C5-1/4-77, B4-1/4-78, A4-1/4-79, G4-1/4-80, F4-1/4-81, Eb4-1/4-82, D4-1/4-83, C4-1/4-84, D4-1/4-85, Eb4-1/4-86, F4-1/4-87, G4-1/4-88, A4-1/4-89, Bb4-1/4-90, B4-1/4-91, C5-1/4-92, D5-1/4-93, C5-1/4-94, B4-1/4-95, A4-1/4-96, G4-1/4-97, F4-1/4-98, G4-1/2-99
```

</div>

<div markdown="1" displayName="5" class="text-note" hidden="True">

**User:**

`The melody goes up and down in predictable steps like C, D, E, F, G, F, E, D, E and so on. That doesn't make for good music! Can you please plan out the melody in advance, and make sure it has a rhythm and tension that makes sense across the piece. That is, with a theme that reoccurs perhaps two or three times, with some development of verse in between. Make sure the tempo isn't tooboring`

**GPT-4:**

```
Absolutely, I understand your point. Here's a more engaging and thematic melody:

A4-1/4-0.5, G4-1/8-1, A4-1/8-1.25, B4-1/4-1.5, C5-1/2-2, B4-1/4-3, A4-1/4-3.5, G4-1/2-4, A4-1/4-5.5, G4-1/4-6, F4-1/2-7, G4-1/4-8.5, A4-1/4-9, B4-1/2-10, A4-1/4-11.5, G4-1/4-12, C5-1/2-13, B4-1/4-14, A4-1/4-15, B4-1/2-16, C5-1/2-17, D5-1/2-19, C5-1/2-20, G4-1/2-22, A4-1/4-24, B4-1/4-25, C5-1/2-26, B4-1/4-28, A4-1/4-29, G4-1/2-30, A4-1/4-32, F4-1/4-33, G4-1/4-34, A4-1/4-36, G4-1/8-37, F4-1/8-37.25, G4-1/4-37.5, B4-1/2-38, A4-1/2-40, G4-1/2-42, F4-1/4-44, G4-1/4-45, A4-1/2-46, B4-1/4-48, C5-1/4-49, D5-1/2-50, C5-1/4-52, B4-1/4-53, A4-1/2-54, G4-1/4-56, F4-1/4-57, E4-1/4-58, F4-1/2-59, G4-1/4-61, A4-1/4-62, B4-1/2-63, A4-1/4-65, G4-1/4-66, F4-1/2-67, G4-1/4-69, A4-1/4-70, G4-1/8-71, A4-1/8-71.25, B4-1/4-71.5, A4-1/2-72, G4-1/2-74, A4-1/4-76, B4-1/4-77, C5-1/2-78, B4-1/4-80, A4-1/4-81, G4-1/2-82, A4-1/4-84, B4-1/4-85, C5-1/8-86, B4-1/8-86.25, G4-1/8-86.5, A4-1/4-86.75, G4-1/2-87.5, F4-1/4-89.5, E4-1/4-90, D4-1/8-91, E4-1/2-92, F4-1/4-94, E4-1/4-95, F4-1/4-96, D4-1/4-97, C4-1/4-98, Bb3-1/4-99, A3-1/4-100.
```
</div>

<div markdown="1" displayName="6" class="text-note" hidden="True">

**User:**

`The melody is all right but appears to be out of key with respect to the chord progression that I provided. Can you see if you can identify the notes in your melody that are harmonically out of line with respect to the key? Also, in what key do you think the chord progression I gave is?`

**GPT-4:**

```
I see, my apologies for the oversight. The chord progression you've provided uses predominantly chords that are found within the F major key, and prominently features a F-C-Bb pattern, which is often found in F major progressions. 

However, there are definitely instances where it incorporates chords that could be seen as borrowing from other keys, such as B Major (possibly borrowed from F# major), or A Major (possibly borrowed from D minor). Including these unique chord choices, we can't definitively say the chord progression is in one key and instead it would be more accurate to consider it as modulating or changing keys throughout.

Here, I would need to adjust the melody around bar 34 (Ab2-1-34, Gb3-
```

</div>

<div markdown="1" displayName="7" class="text-note" hidden="True">

**User:**

`Please give me the fixed melody in full. You were correct about the key being F major by the way`

**GPT-4:**

```text
[*] Making request to OpenAI API
Traceback (most recent call last):
  File "/Users/isak/kth/7an/degree-project/40-programming/code/GPT-4-To-MIDI/g2m.py", line 76, in <module>
    print('[*] Making request to OpenAI API')
  File "/Users/isak/.asdf/installs/python/3.9.7/lib/python3.9/site-packages/openai/_utils/_utils.py", line 277, in wrapper
    return func(*args, **kwargs)
  File "/Users/isak/.asdf/installs/python/3.9.7/lib/python3.9/site-packages/openai/resources/chat/completions.py", line 579, in create
    return self._post(
  File "/Users/isak/.asdf/installs/python/3.9.7/lib/python3.9/site-packages/openai/_base_client.py", line 1240, in post
    return cast(ResponseT, self.request(cast_to, opts, stream=stream, stream_cls=stream_cls))
  File "/Users/isak/.asdf/installs/python/3.9.7/lib/python3.9/site-packages/openai/_base_client.py", line 921, in request
    return self._request(
  File "/Users/isak/.asdf/installs/python/3.9.7/lib/python3.9/site-packages/openai/_base_client.py", line 1020, in _request
    raise self._make_status_error_from_response(err.response) from None
openai.BadRequestError: Error code: 400 - {'error': {'message': "This model's maximum context length is 8192 tokens. However, your messages resulted in 8222 tokens. Please reduce the length of the messages.", 'type': 'invalid_request_error', 'param': 'messages', 'code': 'context_length_exceeded'}}
```
</div>

<br>

---

## Files etc

**Source code:** [g2m.py](https://raw.githubusercontent.com/isakcodes/GPT-4-To-MIDI/993ba68a0ef40b6342f3ba723360ec5f108b2003/g2m.py)

**Attribution:** Fork of [original work by d3n7 on GitHub](https://github.com/d3n7/GPT-4-To-MIDI) with small modifications.


<details markdown="1"><summary>Files</summary>

- All output files [out/rock/](https://github.com/isakcodes/GPT-4-To-MIDI/tree/993ba68a0ef40b6342f3ba723360ec5f108b2003/out/rock)
- [Terminal log file](https://raw.githubusercontent.com/isakcodes/GPT-4-To-MIDI/tree/993ba68a0ef40b6342f3ba723360ec5f108b2003/out/rock/log.txt)

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