<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Verse Player</title>
  <style>
    :root{
      --accent: #0b7285;
      --bg: #f9fafb;
    }
    body{
      font-family: system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background: var(--bg);
      color: #0b0b0b;
      padding: 32px;
      line-height: 1.5;
    }

    /* Clickable block styling */
    .playable {
      display: inline-block;
      padding: 14px 18px;
      border-radius: 10px;
      border: 1px solid rgba(11,114,133,0.12);
      background: white;
      box-shadow: 0 6px 20px rgba(11,114,133,0.04);
      cursor: pointer;
      user-select: none;
      transition: transform .08s ease, box-shadow .12s ease;
    }
    .playable:active { transform: translateY(1px); }
    .playable:focus { outline: 3px solid rgba(11,114,133,0.18); }

    .hint {
      display:block;
      margin-top:8px;
      font-size:0.9rem;
      color: #495057;
    }

    .status {
      margin-left:12px;
      font-weight:600;
      color: #0b7285;
    }

    .glossary {
      margin-top:20px;
      background: #fff;
      padding: 14px;
      border-radius: 8px;
      border: 1px solid rgba(0,0,0,0.04);
    }

    /* Make strong text visually bold if any user agent strips <strong> */
    .playable strong { font-weight: 700; font-size: 1.05rem; }

  </style>
</head>
<body>

  <!-- Playable area: bold paragraph. clickable and keyboard-accessible -->
  <div id="playable" class="playable" role="button" tabindex="0" aria-pressed="false" aria-label="Play verse audio">
    <strong>
      The soul is neither born, nor does it ever die; nor having once existed, does it ever cease to be.
      The soul is without birth, eternal, immortal, and ageless. It is not destroyed when the body is destroyed.
    </strong>
    <span id="status" class="status" aria-live="polite"></span>
    <span class="hint">Click or press Enter/Space to play / pause.</span>
  </div>

  <!-- transliteration / glossary below -->
  <div class="glossary" aria-hidden="false">
    <p><em>Transliteration / word-by-word glossary:</em></p>
    <p>
      na jāyate — is not born; mriyate — dies; vā — or; kadāchit — at any time; na — not; ayam — this; bhūtvā — having once existed;
      bhavitā — will be; vā — or; na — not; bhūyaḥ — further; ajaḥ — unborn; nityaḥ — eternal; śhāśhvataḥ — immortal; ayam — this;
      purāṇaḥ — the ancient; na hanyate — is not destroyed; hanyamāne — is destroyed; śharīre — when the body.
    </p>
  </div>

  <!-- Hidden audio element -->
  <audio id="audio" preload="auto">
    <source src="bgverse20.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>

  <script>
    (function(){
      const playable = document.getElementById('playable');
      const audio = document.getElementById('audio');
      const status = document.getElementById('status');

      function updateStatus(){
        if(audio.paused){
          status.textContent = 'Paused';
          playable.setAttribute('aria-pressed', 'false');
        } else {
          status.textContent = 'Playing';
          playable.setAttribute('aria-pressed', 'true');
        }
      }

      // toggle play / pause
      function togglePlay(){
        if(!audio.src){
          // no source found
          status.textContent = 'Audio not found (place bgverse20.mp3 next to this file)';
          return;
        }
        if(audio.paused){
          audio.currentTime = audio.currentTime || 0;
          audio.play().catch(err => {
            console.error('Playback failed:', err);
            status.textContent = 'Playback blocked — user gesture required';
          });
        } else {
          audio.pause();
        }
        updateStatus();
      }

      // event listeners
      playable.addEventListener('click', togglePlay);
      playable.addEventListener('keydown', function(e){
        // support Enter and Space for keyboard activation
        if(e.key === 'Enter' || e.key === ' ' || e.code === 'Space'){
          e.preventDefault();
          togglePlay();
        }
      });

      // update status when playback state changes
      audio.addEventListener('play', updateStatus);
      audio.addEventListener('pause', updateStatus);
      audio.addEventListener('ended', function(){
        // reset to paused state when finished
        audio.pause();
        audio.currentTime = 0;
        updateStatus();
      });

      // initialize status text
      updateStatus();
    })();
  </script>
</body>
</html>
