# fit-focus-helper

`fit-focus-helper` is a tool which can help to achieve better focus
and collimation while imaging. It can measure various parameters of
stars in the field (sharpness, roundness, half flux
radius). `fit-focus-helper` doesn't acquire images, but waits for them
to appear in a directory (it periodically polls its contents, right
now it doesn't use smarter methods like inotify). The tool is
tested/used with the ASI1600MC and ASI178MM. It is also a quick fits
image browser.

## dependencies

You need to have the following Python libraries installed:

* `pip install numpy`, Numeric Python, for various image operations.

* `pip install opencv-python`, OpenCV, for debayering, color space
  conversion and scaling.

* `pip install astropy`, Astropy, for handling fits files and image
  processing.

* `pip install pycairo`, Cairo, for drawing annotations on images.

* `pip install pygobject`, PyGObjects bindings for Gtk3, GLib and Gdk.

* `pip install photutils`, photutils, for the source detection
  routines.
