# edited-raw-to-jpeg

>   Converts camera RAW or DNG files (including Adobe Camera Raw edits!) to JPEGs

Converts a folder of RAW images to JPEGs and copies to another folder, **macOS only**.
Tested with DNG and CR2 files with XMP sidecars with Adobe Camera Raw edits.

Will attempt to convert all files in the input folder (excluding xmp files of course).

## Requirements

### Adobe DNG Converter
Download it from https://helpx.adobe.com/photoshop/using/adobe-dng-converter.html
The script assumes it is placed in the Applications folder
('/Applications/Adobe DNG Converter.app/Contents/MacOS/Adobe DNG Converter' is run)

See the manual [here](http://wwwimages.adobe.com/www.adobe.com/content/dam/acom/en/products/photoshop/pdfs/dng_commandline.pdf)

## ufraw-batch

```
brew install ufraw-batch
```

Or head to http://ufraw.sourceforge.net/Guide.html

## Usage

```
./dng-to-jpeg INPUT_DIR OUTPUT_DIR
```
eg:

```
./dng-to-jpeg in out
```

## Relies on
- "Adobe DNG Converter", therefore **macOS only**
- ufraw-batch
