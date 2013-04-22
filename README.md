Leaflet.Spin
============

Shows a nice spin cursor on the map.

Requires [Spin.js](http://fgnass.github.com/spin.js/).

See [online demo](http://jsfiddle.net/vsFNC/).


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

    var layer = L.geoJson.ajax();
    layer.addUrl('http://server/path.geojson');

```


Authors
-------

[![Makina Corpus](http://depot.makina-corpus.org/public/logo.gif)](http://makinacorpus.com)
