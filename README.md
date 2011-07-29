This should allow you to automatically start [Voxeo Prism](http://www.voxeo.com/prism/) on Ubuntu.  I have it starting at system boot on Ubuntu 11.04.  YMMV.

*NOTE.* Attempting to run /path/to/prism/bin/prism status tells me that the service control manager isn't running, even though it is.  Assuming the service has actually started correctly I don't think this is a real problem.

## Install

    $ bash < <(curl -s https://raw.github.com/chrisroos/voxeo-prism-ubuntu-startup/master/install)
    
*NOTE.* There are currently warnings from update-rc.d because the scripts are missing some LSB information.  I think this is safe to ignore.

*NOTE.* You'll also get warnings from update-rc.d if the service has already been installed.  I think these are safe to ignore too.