# concatenate-logs

This script will concatenate a set of files, group them by IP address and sort by time resulting in a single file.

## Getting Started
 
Assume you are given the path to a folder and the folder contains 64 files with the approximate size of each file to be 1GB. The output of the script should be a single file containing all the lines from the previous files. The order of the lines in the resulting file should be grouped by IP address and sorted by time within the group.

The names of the files should be of the format: hwFile1.log, hwFile2.log and so on till hwFile64.log
The format of the lines inside the file can be assumed to be the following: 74.125.196.102-- acbonline [22/April/2018:06:25:02 +0000] "GET /xxx/xxx HTTP/1.1" 200 41174 "file:///" "Mozilla/4.0 (compatible; NativeHost)"
The name of the output file should be: hwOutputFile.log

The bash script is saved as firstname.lastname.sh. The script should take 2 arguments, the first parameter will be the path of the folder that has the log files and the second parameter will be the path of the folder where the resulting file will be created.

## Prerequisites

Confirm log file directory exists and files are present

confirm output directory exists

clone repository

## Installation / Usage

Shell Script Usage:
./abdul.sofiz.sh /path/to/logs/directory /path/to/output/directory

## Verify the script worked

cat /path/to/output/directory/hwOutputFile.log to verify

At this point the hwOutputFile.log file should be a single file containing all the lines from the previous files grouped by IP address and sorted by time.


