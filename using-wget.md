# using wget

My wget is in  /usr/bin/wget /usr/share/man/man1/wget.1.gz /usr/share/info/wget.info.gz
My wget version is GNU Wget 1.20.1 built on linux-gnu
There are a crap ton of option flags.  Would not be easy to list them all here.
Note this was only tested by doing `wget` with a upper or lowercase option flag to see what it would return.
There is also a crap ton of `--` flags used.

## Lowercase option flags

`wget -a` says option requires an argument -- `a`. May not exist. Probably actually `-A`

`wget -b` says missing URL. Used to resume interrupted downloads.

`wget -c` says misisng URL. used to continue interrupted downloads, similar to -b

`wget -d` says missing URL. used for directory recursion. It instructs wget to download files and their directory structure recursively from a website.

`wget -e` says option requires an argument -- `e`. used to specify the maximum number of retries for failed downloads.

`wget -h` prints help

`wget -i` says option requires an argument -- `i`. used to download files from a list contained in a text file.

`wget -k` says missing URL. May not exist.  May actually be `-K`

`wget -l` says option requires an argument -- `l`. instructs it to print links found in downloaded HTML files.

`wget -m` says missing URL. used for mirroring, which means creating a local copy of a remote website's directory structure and files

`wget -n` says option requires an argument -- `n`. tells it to not try to clobber existing files

`wget -o` says option requires an argument -- `o`.  used to specify a log file where wget will write information about the download process

`wget -p` says missing URL.  used to specify a log file where wget will write information about the download process. `wget -m -p`

`wget -q` says missing URL. used to suppress the output that wget normally generates during the download process. In other words, it tells wget to operate in quiet mode

`wget -r` says missing URL. used for recursive downloads

`wget -t` says option requires an argument -- `t`. command is used to specify the number of retry attempts for failed downloads. `wget -t 3 http://example.com/file.zip`

`wget -v` says missing URL. instructs it to be verbose during the download process.

`wget -w` says option requires an argument -- `w`. In older versions this specified wait time.  but this may be related to `--warc-file`

`wget -x` says missing URL. used to **force wget to treat the following argument as a list of FTP exclusion patterns.

## Uppercase option flags

`wget -A` says option requires an argument -- `A`. Accept only certain file types

`wget -B` says option requires an argument -- `B` Set the directory prefix to BASE

`wget -D` says option requires an argument -- `D`. Set the directory prefix to BASE

`wget -E` says missing URL. Use server-specified encoding type.

`wget -F` says missing URL. Turn off SSL certificate verification

`wget -H` says missing URL. Enable HTTP proxy support

`wget -I` says option requires an argument -- `I`. Specify URLs to get.

`wget -K` says missing URL Follow redirects

`wget -L` says missing URL. Follow links in HTML instead of downloading the HTML itself

`wget -N` says missing URL. Turn on timestamping.

`wget -O` says option requires an argument -- `O`. Specify the filename for the downloaded content.

`wget -P` says option requires an argument -- `P`. Specify the directory prefix to use when saving locally.

`wget -Q` says option requires an argument -- `Q`. Disable printing of the size of downloadable files.

`wget -R` says option requires an argument -- `R`. Exclude certain files from what gets downloaded.

`wget -S` says missing URL. Turn on logging of all network activity.

`wget -T` says option requires an argument -- `T`. Set modification time of local files.

`wget -U` says option requires an argument -- `U`, Override the User-Agent header sent to the server.

`wget -V` prints version information. Output version information and exit.

`wget -X` says option requires an argument -- `X` Exclude files matching shell pattern from what gets downloaded.

`wget -Y` says option requires an argument -- `Y`. Turn on server-sent event support

wget help is at `wget --help` or `wget -h`

Interesting things to do like download PDF's
wget -r -np -l inf -A pdf -w 1 http://example.com
wget -q --show-progress -r -np -l inf -A pdf -w 1 http://example.com
wget -r -np -l inf -A pdf -w 1 -P /path/to/download/directory http://example.com