# Icon theme carousel arrows

Collection Carousel = Icon theme
To re-position the arrows from the bottom left position to either side of the carousel without any z-index issues:

Add this to the bottom of queries.css.liqiud to over-write the baked in styles

```html
@media screen and (max-width: 740px ) {
    .collection-carousel .owl-controls {
        position: absolute;
        top: 33%;
        width: 120%;
        left: -10%;
        z-index: 0;
    }
    .collection-carousel .owl-wrapper-outer {
        z-index: 1;
    }
    .owl-prev {
        float: left;
    }
    .owl-next {
        float: right;
    }
}
```
