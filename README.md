#### NOTE: This is an unstable development version which has not yet been released, and is not guaranteed to work, do not use.  

For the stable release verision, see: [Latest release](https://github.com/mkillewald/bbslinkwall/releases/latest)

# C-Net BBSLink Wall 2.0.1 (devel version)


A C-Net Pfile used to seamlessly connect a C-Net Amiga BBS to the BBSLink.net networked Grafitti Wall. 
http://www.bbslink.net/sysop/wall.php

![BBSLink.net Wall](http://games.bbslink.net/wall.php)



**************************************************************************

### Changelog

Version 2.0.0 by k1ds3ns4t10n of -X-caliber BBS on 4 Sep 2019
  - Replaced httpj with http_get to resolve stability issues with the BBS locking up when posting.
  - Resolved issue with token expiring before user typed in their wall post.
  - Added showStatus, autoRetry, and logErrors as Sysop configurable switches
                                                                   
Version 1.0.0 written by Link of CheckSum Acknowledged BBS on 3 Feb 2018
  - original version
                                                                   
CheckSum Acknowledged BBS has sadly gone offline as of: 15 Jul 2019  :(                                
                                                                    
Use at your own risk.                                              
**************************************************************************

### Installation Instructions:

1.  Create a folder called 'BBSLink' in your PFiles: directory.
    Copy this file there.
    
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
    
5.  Add a line to your SYSTEXT:sys.welcome file like this:
    
    Q#0 pfiles:bbslink/bbslinkwall}

    ^ NOTE: "Q" here is a ctrl-Q
     
6.  That's it!

**************************************************************************
### -X-caliber BBS telnet://bbs.aholix.net:6800
