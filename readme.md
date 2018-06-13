Sample Usage:

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