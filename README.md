batch-smart-resize
==========
[GIMP](http://gimp.org) script-fu for batch resizing images.
- Maximum height and width can be specified.
- Crops to layer mask.
- Optional padding in any color to the full maximum dimensions.


#### Installation
- Download https://github.com/per1234/batch-smart-resize/archive/master.zip
- Unzip and move the file batch-smart-resize.scm to your GIMP scripts folder. You can find the location of the scripts folder by going to **Edit > Preferences > Folders > Scripts**.
- If GIMP is running click **Filters > Script-Fu > Refresh Scripts**.


<a id="usage"></a>
#### Usage
The script dialog can be accessed at: **File > Create > batch-smart-resize**.
- **Source Folder** - The folder that contains the source images. All files in the folder must be valid image files or the script will fail with the error: `Error: Procedure execution of gimp-file-load failed: Unknown file type`.
- **Destination Folder** - The folder where the processed images will be saved to.
- **Output Filename Modifier** - A string to add to the end of the output filenames.
- **Output Type** - File type to use for the processed images.
- **Output Quality** - Determines the compression level for JPEG Output Type. A higher value will produce better image quality and larger file size.
- **Max Width** - The maximum width of the processed image.
- **Max Height** - The maximum height of the processed image.
- **Pad** - If this box is checked then the script will add background to size the image to the full maximum dimensions. This can be useful to avoid having sites such as Etsy and Handmade at Amazon crop your image thumbnails to an arbitrary aspect ratio.
- **Padding Color** - Color used for padding if enabled.
