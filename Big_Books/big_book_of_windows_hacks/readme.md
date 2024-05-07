big book of windows hacks || big files ... 

... to look in a archive

zcat archive.tar

... to compress a large file for github limit 

tar -czvf - /path/to/files | split -b 40M - archive.tar.gz

Will give you a number of files:

archive.tar.gzaa

archive.tar.gzab

... Which then can be uncompressed with:

cat archive.tar.* | tar -xzvf -
