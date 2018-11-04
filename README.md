# edam

## Overview
1. Raw CR2 files stored on Google Cloud Storage (GCS)
2. Kubernetes (GCP) Elasticsearch install 
3. Elasticsearch listens for GCS file changes
  - dcraw extracts EXIF data from CR2 files, updates indexes
  - ImageMagik regenerates image thumbnails
5. JS frontend queries ES server
6. Add Lightroom export tool to get ratings, collections, links to JPGs

## Research
Detailed info on cr2:
http://lclevy.free.fr/cr2/

c-library to decode raw files, dcraw:
http://www.cybercom.net/~dcoffin/dcraw/

Show metadata from a file:
dcraw -i -v ~/Pictures/2017/2017-02-04/MR2A0699.CR2

ImageMagik/dcraw Docker image:
e.g.: https://github.com/dooman87/imagemagick-docker/blob/master/Dockerfile

Export Metadata commercial plugin:
https://exchange.adobe.com/addons/products/2356
