# gns3feed - generate ATOM/RSS feed from GNS3 community website

gns3feed connects to the GNS3 community website and
creates an ATOM/RSS feed from it.

It requires Python 3 and the feedgen and requests modules.
These can be installed with `pip3 install feedgen` and
`pip3 install requests`.

#### Usage

```text
gns3feed [-h] [-v] [-a file] [-r file]

optional arguments:
  -h, --help, -?        prints this screen
  -v, --version         prints version
  -a file, --atom file  generate ATOM feed
  -r file, --rss file   generate RSS feed
```

Run this program regulary, for example by cron, and
add the generated feed file to your newsfeed reader.

Currently this program is highly experimental.
It will break anytime the GNS3 website changes it's structure.
Furthermore it got very limited testing, mainly with Vienna,
a RSS/Atom reader for macOS.
