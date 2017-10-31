# jquery, jquery.autosave - SPIP 3.1.x and above
Canonicalize javascript prive/javascript/jquery.autosave.js
using [jsDelivr Github CDN](https://www.jsdelivr.com/feature) and [mod_pagespeed](https://github.com/pagespeed/mod_pagespeed).

## Apache pagespeed.conf:

This will enable canonicalization for jquery.js (1.12.4 in SPIP 3.1.x) using googleapi CDN :
 ```
 ModPagespeedEnableFilters canonicalize_javascript_libraries
 ```
 Adding this :
 ```
 ModPagespeedLibrary 741 Ppl_Ry-HtT_ZvQ-n3zm_Q \
 //cdn.jsdelivr.net/gh/opalesurfcasting/jquery.autosave@v1.0/jquery.autosave.min.js
 ```
 will enable canicalization for jquery.autosave.js
 
## Direct urls :
 
 raw : https://cdn.jsdelivr.net/gh/opalesurfcasting/jquery.autosave@v1.0/jquery.autosave.js
 
 minified : https://cdn.jsdelivr.net/gh/opalesurfcasting/jquery.autosave@v1.0/jquery.autosave.min.js
