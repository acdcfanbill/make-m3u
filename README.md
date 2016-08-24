# make-m3u
## About
This is a small shell program to generate a m3u playlist from a given
folder.  It will search the current directory for files ending in a
specific extension (mp3 by default) and then sort that list and generate
a m3u file from it.  It will return all text to std out by default, or
you can specify a output filename.  You can also give it a list of files
and ask it to sort them, or take them as they are and make a m3u out of
those.

## Requirements
python2, and pymediainfo to pull the arist and track name from the files

## Usage
    Usage: make-m3u [options] file1 file2 file3 ...
            The program will search the cwd for files with the given extension
            (mp3 by default) or take the list of files from the arguments and
            build a m3u out of them.
    
    Options:
      -h, --help            show this help message and exit
      -o OUTFILE, --output-file=OUTFILE
                            Output file to write to, otherwise prints to std out
      -e EXTENSION, --file-extension=EXTENSION
                            File extension to match, defaults to mp3
      -s, --sort            Sort the list of files you use as arguments
                            (default=False). Getting files from cwd will always
                            sort them based on file name.

## Other
Last updated: 20160824

Python script by acdcfanbill

This script is distributed in the hope that it will be useful,  
but WITHOUT ANY WARRANTY; without even the implied warranty of   
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
