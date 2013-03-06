Leaflet.Spin
============

Shows a nice spin cursor on the map.

Requires [Spin.js](http://fgnass.github.com/spin.js/)

Usage
-----

```

    var layer = L.GeoJSON(null).addTo(map);
    
    layer.fire('data:loading');
    $.getJSON('http://server/path.geojson', function (data) {
        layer.fire('data:loaded');
        layer.addData(data);
    });

```
