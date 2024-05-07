---
layout: post
title:  "Chordinator sample chord progressions"
date:   2024-05-04 22:09:51 +0200
categories: chordinator
---

<h1>Sample Chordinator chord progressions</h1>
<div id="listening-area-1" class="listening-area">
  <div class="tab"></div>
  <div id="player">
    <p class="helptext">Select one of the tabs, then press play to listen.</p>
    <midi-visualizer type="piano-roll" id="mainVisualizer" src=""></midi-visualizer>
    <midi-player src="" sound-font visualizer="#mainVisualizer" id="mainPlayer"></midi-player>
  </div>
  <div id="files-list-area">
    <h2>Files</h2>
    <ul class="midifiles">
      <li><a class="afile" displayName="Blues" href="{{ '/assets/chordinator_samples/163418_23_3_2024_generated_Blues.mid' | relative_url }}">Blues (163418_23_3_2024_generated_Blues.mid)</a></li>
      <li><a class="afile" displayName="Rock" href="{{ '/assets/chordinator_samples/155747_23_3_2024_generated_Rock.mid' | relative_url }}">Rock (155747_23_3_2024_generated_Rock.mid)</a></li>
      <li><a class="afile" displayName="Jazz 1" href="{{ '/assets/chordinator_samples/160411_23_3_2024_generated_Jazz.mid' | relative_url }}">Jazz 1 (160411_23_3_2024_generated_Jazz.mid)</a></li>
      <li><a class="afile" displayName="Jazz 2" href="{{ '/assets/chordinator_samples/160810_23_3_2024_generated_Jazz.mid' | relative_url }}">Jazz 2(160810_23_3_2024_generated_Jazz.mid)</a></li>
      <li><a class="afile" displayName="Jazz 3" href="{{ '/assets/chordinator_samples/161405_23_3_2024_generated_Jazz.mid' | relative_url }}">Jazz 3(161405_23_3_2024_generated_Jazz.mid)</a></li>
      <li><a class="afile" displayName="Jazz 4" href="{{ '/assets/chordinator_samples/161602_23_3_2024_generated_Jazz.mid' | relative_url }}">Jazz 4(161602_23_3_2024_generated_Jazz.mid)</a></li>
      <li><a class="afile" displayName="Jazz 5" href="{{ '/assets/chordinator_samples/161808_23_3_2024_generated_Jazz.mid' | relative_url }}">Jazz 5(161808_23_3_2024_generated_Jazz.mid)</a></li>
      <li><a class="afile" displayName="Jazz 6" href="{{ '/assets/chordinator_samples/161915_23_3_2024_generated_Jazz.mid' | relative_url }}">Jazz 6(161915_23_3_2024_generated_Jazz.mid)</a></li>
      <li><a class="afile" displayName="Jazz 7" href="{{ '/assets/chordinator_samples/162708_23_3_2024_generated_Jazz.mid' | relative_url }}">Jazz 7(162708_23_3_2024_generated_Jazz.mid)</a></li>
    </ul>
  </div>
</div>

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

/*
  var downloadsTab = document.createElement('button');
  downloadsTab.textContent = "Downloads"
  downloadsTab.onclick = function(event) {
    displayDownloads(event);
  };
  tab.appendChild(downloadsTab); */
});

/*function displayDownloads(event) {
  var fileslist = event.currentTarget.parentElement.parentElement.querySelector('#files-list-area');
  var downloadTabContent = event.currentTarget.parentElement; //.parentElement.querySelector('#files-list-area');
  console.log(fileslist)
}*/

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
}
</script>
{% endraw %}