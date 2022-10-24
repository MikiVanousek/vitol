# Get Satellite Imagery by Geographic Coordinates

Download Google Maps satellite images of any resolution by geographic coordinates.

![](examples/img_1.png)
<sub><sub>© 2022 Google<sub><sub>

## Usage

>Note that `main.py` implements the interface, so if you only need the image generation function, go to `image_generation.py`.

Install the required packages.<br>
```console
pip install -r requirements.txt
```
Run `main.py`.

### Preferences file
If there is no `preferences.json` file, a default one will be created.

* `"url"` is the url template that the script is using to get map tiles. The default url may no longer work, so you may have to obtain a new one (if you are using Google Chrome, [this article](https://developer.chrome.com/docs/devtools/network/) should help) and replace its x, y and z values with `{x}`, `{y}` and `{z}`.
* `"dir"` is the directory where new images will be saved.
* `"region_ul"` and `"region_br"` are comma-separated coordinates of the upper-left and bottom-right corner of the region. Leave theese empty to enter the coordinates in terminal.
* `"zoom"` is the zoom level. At each zoom level, there is four times as many 256x256 tiles in a region as at the previous zoom level.
* `"headers"` are the HTTP headers that the script is using.

---
## Examples

![](examples/img_2.png)
<sub><sub>© 2022 Google<sub><sub>
<br><br>

![](examples/img_3.png)
<sub><sub>© 2022 Google<sub><sub>
<br><br>

![](examples/img_4.png)
<sub><sub>© 2022 Google<sub><sub>
