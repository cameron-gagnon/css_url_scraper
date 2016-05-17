# URL_SCRAPER

python3.5 is what this was written in, but most python3.x's should work.

To install the dependencies: `pip install -r requirements.txt`
It only relies on the `requests` library.

### Assumptions made in order to work:
1. Make sure you are above the `styles` directory where the `css` files are that you wish to download from. The general structure is that your `fonts`,`images`, and `scripts` directories are next to the `styles` one. If the `fonts` and `images` directories are not yet created, this script will create and fill them with the relevant files (ex. `.png` files will go in `images` folder).
2. You must replace the `DOMAIN` variable at the top of the script to the appropriate value. Generally an `href` in the `<script>` tag of an `html` file will have the `DOMAIN` that it is pulling the resources from. If the `DOMAIN` is specified in all `url(...)`'s then leave `DOMAIN` blank.


This script will download the file in the path `url('/remote/path/to/asset.png')` in all files under the `styles` folder and place it into either `fonts` or `images` if it is a font or image respectively. It will then update the path it downloaded the file from to be the new local path to the file.


Most errors should be presented in red output,
otherwise, all successful downloads should be presented in a
yellowish-green text depending on your color settings.
