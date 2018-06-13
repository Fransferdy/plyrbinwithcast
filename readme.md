# This is a distribution of sampotts/plyr with a working chrome cast feature (by guruparas), built with the most recent plyr up to April 30th 2018.

https://github.com/sampotts/plyr
https://github.com/gurupras/plyr/tree/chromecast


# Sample Usage:

```javascript

<script src="./plyr/plyr.js?v=<?php echo SITE_VER;?>"></script>
<link href="./plyr/plyr.css" rel="stylesheet">

<script>

var myControls = ['play-large', 'play', 'progress', 'current-time', 'mute', 'volume', 'captions', 'settings', 'pip', 'airplay', 'fullscreen'];
if (window.chrome)
{
    myControls[myControls.length] = 'googlecast';
}

const player = new Plyr('#videoplayer',
{
iconUrl:'plyr/plyr.svg',
controls: myControls
});

</script>

```
