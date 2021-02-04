how to use

# How to use

run `npm i` to install the node_modules dependencies

run `npm serve` to launch the development server

visit `http://localhost:8080` to view live changes

## How it works

thumbnails are generated using a node.js library called sharp
https://github.com/lovell/sharp

the thumbnails are automatically saved in a `thumb` folder

The HTML is dead simple

```
<a href="{{image}}" class="glightbox" data-gallery="gallery1">
    <img src="thumb/{{image}}"/>
</a>
```

The lightbox is GLightbox which is self hosted inside `assets/js/glightbox.min.js`
see `base.njk` for `<script src="/assets/js/glightbox.min.js" ></script>`
