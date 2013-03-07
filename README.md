Leaflet.Spin
============

Shows a nice spin cursor on the map.

Requires [Spin.js](http://fgnass.github.com/spin.js/)

Usage
-----

### With JQuery

```

    var layer = L.geoJson(null).addTo(map);
    
    layer.fire('data:loading');
    $.getJSON('http://server/path.geojson', function (data) {
        layer.fire('data:loaded');
        layer.addData(data);
    });

```

### With [Leaflet.AJAX](https://github.com/calvinmetcalf/leaflet-ajax/)

```

    var layer = new L.GeoJSON.AJAX();
    
    layer.on('beforeDataLoad',   function() { layer.fire('data:loading'); });
    layer.on('dataLoadComplete', function() { layer.fire('data:loaded'); });
    
    layer.addUrl('http://server/path.geojson');

```
