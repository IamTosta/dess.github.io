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

  
</body>
</html>
