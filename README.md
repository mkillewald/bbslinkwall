### NOTE: This is an unstable development branch which has not yet been released, and is not guaranteed to work. Do not use this version, you have been warned.

### For the stable release verision, return to branch [master](https://github.com/mkillewald/bbslinkwall/tree/master), or download the [latest release](https://github.com/mkillewald/bbslinkwall/releases/latest)

# C-Net BBSLink Wall 2.0.1 (devel version)


A C-Net Pfile used to seamlessly connect a C-Net Amiga BBS to the BBSLink.net networked Graffiti Wall.
http://www.bbslink.net/sysop/wall.php

![BBSLink.net Wall](http://games.bbslink.net/wall.php)



**************************************************************************

### Changelog
  v2.0.1 (2 Nov 2019) by k1ds3ns4t10n of -X-caliber BBS
   - Code cleanup and refactor
   - Renamed g.logErrors switch to g.debug
   - Added g.defaultResponse and g.showCustomHeader switches
   - Added c.default and c.highlight colors as options
   - Added custom header files with 40/80 column support
   - Added URL encoding

 v2.0.0 (4 Sep 2019) by k1ds3ns4t10n of -X-caliber BBS
  - Replaced httpj with http_get to resolve stability issues with the BBS locking up when posting.
  - Resolved issue with token expiring before user typed in their wall post.
  - Added showStatus, autoRetry, and logErrors as Sysop configurable switches

 v1.0.0 (3 Feb 2018) by Link of CheckSum Acknowledged BBS
  - original version

CheckSum Acknowledged BBS has sadly gone offline as of: 15 Jul 2019  :(

Use at your own risk.
**************************************************************************

### Installation Instructions:

1.  Create a folder called 'BBSLink' in your PFiles: directory.
    Copy this file and the *.wallHeader files there.

2.  Download http_get from Aminet and install in C:

    https://aminet.net/package/comm/tcp/http_get

3.  Register on bbslink.net as a sysop.  If you have already done
    so when you registered for the door game server, you will need
    to use the information you got from that time you registered.

4.  You will receive an email from them with your System Code,
    Authorization Code, and Scheme Code. Copy and paste these values
    from that email into these fields in the bbslinkwall script:

    b.SystemCode='yoursystemcode'
    b.AuthorizationCode='yourauthcode'
    b.SchemeCode='yourschemecode'

5.  Optional: There are several options you may change based on your
    needs in the SysOp Configurable Options block below.

6.  Add this file as an Arexx executable anywhere on your system using
    the path:

    pfiles:bbslink/bbslinkwall

7.  That's it!

**************************************************************************
### -X-caliber BBS telnet://bbs.aholix.net:6800
