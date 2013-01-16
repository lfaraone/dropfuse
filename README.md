dropfuse
========

1. Install: python-fuse, multiprocessing, pyquery
2. Get a link to a Dropbox linked folder
3. Extract the contents of this software and navigate to the software
    folder in command-line.
4. Create an empty directory used during mounting the remote folder,
    for instance : mkdir mnt
5. Run the command:

    python dropfuse.py <dropboc.com url> mnt/

To get you started, I have created a public folder link that you can
test this on:

    https://www.dropbox.com/s/c6ecc2plwconh5x


At this moment if everything goes well, you should see a drive mounted
and named 'mnt'. Open it and use it in a file browser.

To stop using the mounted drive type:

    fusermount -u mnt/

or:

    umount mnt/


Dropfuse will attempt to cache every single item in the folder. It will do so
blindly, without any limits thus caution has to be exercised what size of file
it is used for. Positive trade-off is that audio/video playback is
butter-smooth, caching options will be provided in future enhancements.

