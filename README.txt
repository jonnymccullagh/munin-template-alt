==============================================================================
Munin Template Alternative
==============================================================================
Author: Jonny McCullagh
Date:   12th August 2013
==============================================================================

DESCRIPTION
------------------
I found a download for an improved Munin layout at:
http://www.mabishu.com/blog/2010/03/24/improve-munin-stats-page-with-new-layout-and-plugins/
However I found there was some missing styles.
I have taken that download as a starting point and spent a few hours
adding a few CSS rules to fix the layout. My additions are
at the top of the style.css file and Mabishu's CSS is below.
I have made very few changes to the original tmpl files to keep things simple.
I have also added a wee Munin raven icon.

INSTALLATION
------------------
- Move to your Munin configuration directory e.g.
        cd /etc/munin
- Extract the tar file contents - you should see a directory named templates_new
- Move your current templates directory e.g.
        mv ./templates ./templates_default
- Move the new templates directory into place
        mv ./templates_alt ./templates
- Move to your munin www directory e.g.
        cd /var/www/munin
- Remove the existing css, and image files (if present)
        rm ./style.css ./logo.png ./favicon.ico
- Wait five minutes and check that the new template is being used. If there
  are any problems check the source for broken paths.

LICENSE
------------------
This program is free software; you can redistribute it and/or modify it under
the terms of the GNU General Public License version 2 as published by the
Free Software Foundation.

==============================================================================
Have fun!
==============================================================================
