# Timeline control

Timeline control allows playing datetimes as animation with linear interpolation between two subsequent datetimes

```javascript
import * as WeatherLayers from '@weatherlayers/weatherlayers-gl';

WeatherLayers.setClientConfig({
  accessToken: 'xxx',
});

const timelineControl = new WeatherLayers.TimelineControl({
  dataset: ..., // string (STAC Collection ID)
  datetime: ..., // string (ISO 8601 datetime)
  datetimeInterpolate: ..., // boolean
  width: ..., // number
  onUpdate: event => {
    console.log(event.datetime); // string (ISO 8601 datetime)
  },
});
```

![](../../../.gitbook/assets/timeline-control.png)