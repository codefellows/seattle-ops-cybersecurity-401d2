# Ops Challenge - File Encryption Script Part 2 of 3

## Demo Code

The demo code below introduces concepts necessary to complete the challenge.

```python

#Import os module
import os
#Import math and time module
import math,time

#Set listing start location
start_path = "C:\Samples"
dir_count = 0
file_count = 0

#Traverse directory tree
for (path,dirs,files) in os.walk(start_path):
    print('Directory: {:s}'.format(path))
    dir_count += 1
    #Repeat for each file in directory
    for file in files:
        fstat = os.stat(os.path.join(path,file))

        # Convert file size to MB, KB or Bytes
        if (fstat.st_size > 1024 * 1024):
            fsize = math.ceil(fstat.st_size / (1024 * 1024))
            unit = "MB"
        elif (fstat.st_size > 1024):
            fsize = math.ceil(fstat.st_size / 1024)
            unit = "KB"
        else:
            fsize = fstat.st_size
            unit = "B"

        mtime = time.strftime("%X %x", time.gmtime(fstat.st_mtime))

         # Print file attributes
        print('\t{:15.15s}{:8d} {:2s} {:18s}'.format(file,fsize,unit,mtime))
        file_count += 1
 # Print total files and directory count
print('\nFound {} files in {} directories.'.format(file_count,dir_count))

```
