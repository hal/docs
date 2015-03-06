# Look &amp; Feel 

### Widgets

HAL builds on the default [GWT widgets][1], with minor modifications to provide a consistent look&amp;feel (css references, image bundles, etc)

For specific interaction types we've implemented dedicated widgets, that go beyond what GWT has to offer. I.e. the form input widget that provides an open-save-close model is good example of this.

If a widget has a general purpose then it belongs into the [Ballroom library][2]. If a widget only serves our very specific project needs, we keep it within the core/gui module.

### Look &amp; Feel

HAL provides two different themes: The default one is the community look&amp;feel used with Wildfly. It's enabled and used out of the box. In order to switch to the product look&amp;feel, you need to rebuild the web console using the `-Peap` maven profile. This will create a console build that relies on the [RCUE][3] styles.

The themes are driven by a [Less CSS][4] build step that creates two distinct css file for inclusion with the final console.

### Accessibility

The web console implements the [W3C Aria specification][5] that defines a way to make Web content and Web applications more accessible to people with disabilities.

The overall layout and each specific [widgets are designed][6] to be composed and provide keyboard access and screen reader support across the board.

It is an important requirement to pass the [508 compliance][7] tests. Please keep this in mind when developing new widgets, layout types or navigation concepts.

[1]: http://www.gwtproject.org/doc/latest/RefWidgetGallery.html
[2]: https://github.com/hal/ballroom
[3]: http://uxd-rcue.rhcloud.com
[4]: http://lesscss.org
[5]: http://www.w3.org/WAI/intro/aria
[6]: http://www.w3.org/TR/wai-aria-practices/
[7]: https://www.section508.gov
  