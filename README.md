# jquery, jquery.autosave - SPIP 3.1.x and above
Canonicalize javascript prive/javascript/jquery.autosave.js
using [jsDelivr Github CDN](https://www.jsdelivr.com/feature) and [mod_pagespeed](https://www.modpagespeed.com/doc/filter-canonicalize-js).

## In Apache pagespeed.conf:

This will enable canonicalization for jquery.js (1.12.4 in SPIP 3.1.x) using googleapi CDN - The parameter below will enable detection from this librarie size and checksum - [canonicalized libraries list](https://github.com/pagespeed/mod_pagespeed/blob/master/net/instaweb/genfiles/conf/pagespeed_libraries.conf) :
 ```
 ModPagespeedEnableFilters canonicalize_javascript_libraries
 ```
 Adding this  :
 ```
 ModPagespeedLibrary 741 Ppl_Ry-HtT_ZvQ-n3zm_Q \
 //cdn.jsdelivr.net/gh/opalesurfcasting/jquery.autosave@v1.0/jquery.autosave.min.js
 ```
 will enable canicalization for jquery.autosave.js, also based on file size 741 and checksum. This is needed as this file is not in default mod_pagespeed [canonicalized libraries list](https://github.com/pagespeed/mod_pagespeed/blob/master/net/instaweb/genfiles/conf/pagespeed_libraries.conf).
 
## Direct urls :
 
 raw : https://cdn.jsdelivr.net/gh/opalesurfcasting/jquery.autosave@v1.0/jquery.autosave.js
 
 minified : https://cdn.jsdelivr.net/gh/opalesurfcasting/jquery.autosave@v1.0/jquery.autosave.min.js
 
 ## Notes :
 
 - Canonicalized libraries will not be combined or minifyed. It's up to you to check what is the best.
