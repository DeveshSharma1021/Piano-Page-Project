# Piano-Page-Project
This project is a simple piano -page project built using HTML, CSS, and JavaScript. It mimics the look and feel of a real piano and allows users to click on keys to play musical notes.

1. HTML (index.html)
Defines the layout of the page:

 (<h1>Piano-Page</h1>)

 <div> container for piano keys.

Each key is a <div> with a data-note attribute (e.g. data-note="C").

 No actual sound is embedded in HTML — it's all driven by JavaScript.

2. CSS (style.css)
Styles the piano to look realistic:

White keys: Wide and tall.

Black keys: Narrower, overlaid on white keys using position: absolute.

Key press animations using :active.
Enhances user experience visually and interactively.

3. JavaScript (script.js)
Adds interactivity:

Detects clicks on keys.

Retrieves the data-note from the key.

Plays the corresponding audio file using the Audio object.

javascript
Copy
Edit
const audio = new Audio(`tunes/${note}.mp3`);
audio.play();
Links UI actions to sound playback.

4. Sounds (/sounds folder)
Contains .mp3 tunes files named after notes:
;.mp3, a.mp3, d.mp3, etc.
These are the actual note recordings that play when users interact with the keys.
