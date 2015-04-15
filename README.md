# <img src="http://www.officialpsds.com/images/thumbs/Soundcloud-Logo-psd47614.png" width="75" align="left">&nbsp;react-soundplayer

![](http://img.shields.io/badge/Status-Work%20In%20Progress-brightgreen.svg?style=flat)

> Create highly-customizable SoundCloud players with React.

![](https://dl.dropboxusercontent.com/u/100463011/react-soundplayer-screen.png)

```
npm install react-soundplayer --save
```

## Usage

### Using _with_ [SoundCloudAudio](https://github.com/voronianski/soundcloud-audio.js)

This way you have benefit of global singleton audio object.

```javascript
import React from 'react';
import ReactSoundPlayer from 'react-soundplayer';

import { SimplePlayer, CoverPlayer } from 'react-soundplayer/components';

const streamUrl = 'https://api.soundcloud.com/tracks/194964548/stream';

let { SoundCloudPlayer } = new ReactSoundPlayer('YOUR_CLIENT_ID');

// <SoundCloudPlayer streamUrl={streamUrl} playerType="simple" />
```

### Using _without_ [SoundCloudAudio](https://github.com/voronianski/soundcloud-audio.js)

```javascript

class AppPlayer extends React.Component {
    render() {
        <div>
            <SoundPlayerComponent>
                
            </SoundPlayerComponent>
        </div>
    }
}
```

---
