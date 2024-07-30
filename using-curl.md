# using curl

`curl -a` says no URL specified. Show error message for server errors. This is used to display error messages returned by the server, which can be helpful for debugging.

`curl -b` says option -b: requires parameter. POST data. Sends the specified data in a POST request. Requires a parameter specifying the data to send.

`curl -c` says option -c: requires parameter. Copy header to stdout. Copies the header sent by the server to standard output. Requires a parameter specifying the file to save the header to.

`curl -d` says option -d: requires parameter. Data to POST. Sends the specified data in a POST request. Requires a parameter specifying the data to send.

`curl -e` says option -e: requires parameter. SSL certificate. Specifies the path to an SSL certificate to use for the connection. Requires a parameter specifying the path to the certificate.

`curl -f` says no URL specified. Fail silently. Fails silently on server errors. This means that curl won't output anything if the server returns an error status.

`curl -g` says no URL specified. Allow trailing slashes in URL. Allows curl to append a slash to the URL if it doesn't already end with one.

`curl -h` prints help

`curl -i` says no URL specified. Include header in output. Includes the header sent by the server in the output.

`curl -j` says no URL specified. Return content only. Returns only the body of the document, excluding the HTTP header.

`curl -k` says no URL specified. Allow connections to SSL sites without certificates. Disables certificate verification.

`curl -l` says no URL specified. Maximum time in seconds that you allow the whole operation to take. Requires a parameter specifying the maximum time allowed.

`curl -m` says option -m: requires parameter. Maximum time in seconds that you allow the whole operation to take. This is similar to -l but is deprecated.

`curl -n` says no URL specified. Don't use SSL certificates. Disables SSL certificate verification.

`curl -o` says option -o: requires parameter. Write output to file instead of stdout. Requires a parameter specifying the file to write the output to.

`curl -p` says no URL specified. Preserve local timestamps. Preserves the modification timestamp when uploading files.

`curl -q` says no URL specified. Quiet mode. Mutes curl's progress meter and error messages.

`curl -r` says option -r: requires parameter. Remote time. Shows the time taken for the entire operation.

`curl -s` says no URL specified. Silent mode. Turns off the progress meter and error messages.

`curl -t` says option -t: requires parameter. Time consumption. Shows the time taken for the entire operation.

`curl -u` says option -u: requires parameter.  User+password for server authentication. Requires a parameter specifying the username and password in the format username:password.

`curl -v` says no URL specified. Verbose. Makes the operation more talkative.

`curl -w` says option -w: requires parameter. Format the output. Requires a parameter specifying the format of the output.

`curl -x` says option -x: requires parameter. Proxy. Specifies the proxy to use for the request. Requires a parameter specifying the proxy address.

`curl -y` says option -y: requires parameter. Trust annotations in peer certificate. Enables trust annotations in peer certificates.

`curl -z` says option -z: requires parameter. Time zone. Specifies the time zone to use for calculating elapsed time. Requires a parameter specifying the time zone.

`curl -M` prints the manpage / help and command usage; same as curl --manual or curl --help.
`curl -V` prints the version. mine is curl 7.64.0

All of the uppercase option flags exist, except -W and -Z.  They might be duplicates of the lowercase option flags.