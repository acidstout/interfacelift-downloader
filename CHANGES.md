## Changes

2019-04-26, acidstout:
* moved user-agent into variable and updated it to something more recent.
* use HTTPS to connect to server.
* default to one thread to avoid hammering the site.
* added variable delay (starts with two seconds) between downloads to avoid hammering the site.
* check for zero-sized files prior download and remove them.
* check type of downloaded files and if they are not valid images remove them. InterfaceLIFT returns HTML page on HTTP errors without sending proper HTTP error code.
* retry download on error
