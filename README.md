# edam

## Overview
1. Raw CR2 files stored on local filesystem - prefereably a NAS
2. Elasticsearch based server runs locally, indexes all metadata
3. Logstash indexes new/changed files -> ES
4. JS frontend queries ES server
5. Add Lightroom export tool to get ratings, collections, links to JPGs
