# Tar files and tar.gz files should be .gz.tar files!
Out of history we got everything wrong in the Community because we did hurry to much.
Tar is a Container format for multiple files while zip is a single stream that leads 
to the conclusion ok i tar my files to save the tree and file attributes so the 
structure so i create a tar file and then zip that. 

But this is highly inefficent! At Runtime as also in transport the correct method
that works at scale is the exact oposit of that as tar leaks integrity checks and zip 
does also the combination of .gz.tar is what we should aim for.

The tar Container Format chunks files into 512b blocks and adds meta data.
the zip format is a compression format for storage efficency. so adding a header on top
of a zip file via tar and a additional related checksums file gives us the best out of all worlds.

This is what we use internal to deliver our own packages in the so called .esar format it is a bit like
asar form electron but implemented to run in any WInterOP Environment. It adds a Stub on top of any data
to identify and load it directly. The stub it self is analyzeable so you can filter out bad actors. 
