# edam

## Overview
1. Raw CR2 files stored on local filesystem - prefereably a NAS
2. Elasticsearch based server runs locally, indexes all metadata
3. Logstash indexes new/changed files -> ES
4. JS frontend queries ES server
5. Add Lightroom export tool to get ratings, collections, links to JPGs

## Research
Detailed info on cr2:
http://lclevy.free.fr/cr2/

c-library to decode raw files, dcraw:
http://www.cybercom.net/~dcoffin/dcraw/

Show metadata from a file:
dcraw -i -v ~/Pictures/2017/2017-02-04/MR2A0699.CR2

Export Metadata commercial plugin:
https://exchange.adobe.com/addons/products/2356
