# Welcome
Welcome to the CORAL-CWS GitHub page. This is the home for a number of tools that we use. General notes about each tool can be found in this file, and more detailed ones can be found in the corresponding repository.

## About CORAL-CWS

TODO Norma: this is a good place to put a public-facing blurb on the team as a whole.

Link to website: https://www.poscanada.org/ ?

Logos are also a good idea.

It'd probably be more convenient for us if this section is moved until just after the "Dependencies" section, but as this is eventually intended to be public facing, I think keeping this brief but at the top is best. You could still have sections further down such as "acknowledgements" or "research details"

## Getting Started
Tools on this page can be downloaded either by either cloning them with Git or by downloading them as a zip. The first method takes a bit more setup as you'll need to install Git, but it makes it very easy to update the tools. The second method is an easy way to access the smaller tools (such as the file management ones), but isn't recommended for any tools that are likely to be updated in the future (such as the AIS_Linker).

## List of Tools
This section provides a brief overview of the tools that are provided on github.

Most of our completed tools are publicly available, and can be downloaded without logging in. If you are part of our team and need access to any of the private tools, please contact Patrick or Gregory to get your github account linked to our team.

### AIS_Linker (private)
TODO

It is recommended to use the image_copy_sort, time_fixer, and _________ tools *before* using the AIS_linker to process images.

### Image copy/sort (private)
This tool copies images between locations, organizing them into daily folders as it does so.

### Other Tools (private)
This is a collection of small tools that don't fit into any other repository. More information on each can be found there. Currently, this list includes:
 * file counter: a PyQt program that lists the number of files in each folder. Useful in searching for anomalies in a repetitive file structure, such as when data is organized into daily folders, each of which should have a comparable amount of data files.
 * file list/copy tool:
 * image_sampler: Specific to our standard image file structure, this tool copies 4 images at specific times each day to a new folder. This is useful when assessing weather conditions or camera status.
 * metadata copier: This tool supports one of our auto-detection tools by searching for duplicate images with metadata missing, then searching for an original image for each duplicate to mirror the metadata over from.

### Other Scripts (private)
This is a collection of scripts that have been used to process AIS data in the past. Many of them are ad-hoc and not intended for re-use, but they may be useful as references for future AIS processing scripts.

## Dependencies
Most of these tools are written in Python 3. Some require additional libraries, the main two of which are:
1. PyQt5 is required for any tool that has a visual interface. It can be installed using pip: "pip install PyQt5"
    - this package is licenced under the GNU General Public Licence. For more details, see the licencing information below.
2. Pillow is used to get image metadata in a number of the correction tools. It can also be installed using pip: "pip install Pillow"

## Licencing information
All of these projects are licenced under the GNU GPLv3 copy-left licence. Details on the permissions of this licence can be found at <https://www.gnu.org/licenses/>.
