<html lang='en'>
    <div id="center">
<div class="dess">
<img alt="Red guitar" src="guitar.gif">
</div>
</div>
<style>
  .dess {
    min-width: 320px;
    max-width: 100%;
    min-height: 320px;
    max-height: 100%;
    position: relative;
    color: black;
    cursor: pointer;
  }
  .dess img {
    position: absolute;
    height: 100%;
    width: 100%;
    object-fit: contain;
    image-rendering: pixelated;
  }
</style>
<script>
  var dess = new Howl({
    src: ['find_her.ogg.mp3', '/assets/audio/findher.mp3'],
    volume: 0.5,
    loop: true
  });
  
  $(document).on('click', '.dess:not(.playing)', function() {
    dess.play();
    $('.dess').addClass('playing');
  });
  
  $(document).on('click', '.dess.playing', function() {
    dess.stop();
    $('.dess').removeClass('playing');
  });
</script>

  </main>
  <script defer>if(!window.plausibleloaded){window.plausibleloaded=true;var onloadfunc = function() {!function(){"use strict";var t=window.location,e=window.document;function a(t,e){t&&console.warn("Ignoring Event: "+t),e&&e.callback&&e.callback()}function n(n,i){if(/^localhost$|^127(\.[0-9]+){0,2}\.[0-9]+$|^\[::1?\]$/.test(t.hostname)||"file:"===t.protocol)return a("localhost",i);if(window._phantom||window.__nightmare||window.navigator.webdriver||window.Cypress)return a(null,i);try{if("true"===window.localStorage.plausible_ignore)return a("localStorage flag",i)}catch(r){}var l={},o=(l.n=n,l.u=t.href,l.d="deltarune.com",l.r=e.referrer||null,i&&i.meta&&(l.m=JSON.stringify(i.meta)),i&&i.props&&(l.p=i.props),new XMLHttpRequest);o.open("POST","https://plausible.fangamer.eu/api/event",!0),o.setRequestHeader("Content-Type","text/plain"),o.send(JSON.stringify(l)),o.onreadystatechange=function(){4===o.readyState&&i&&i.callback&&i.callback()}}e.currentScript;var i=window.plausible&&window.plausible.q||[];window.plausible=n;for(var r,l=0;l<i.length;l++)n.apply(this,i[l]);function o(){r!==t.pathname&&(r=t.pathname,n("pageview"))};o();}();}; onloadfunc();}</script>
  
</body>
</html>
