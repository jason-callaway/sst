SST Security Toolkit
====================

**Note**: This project is not being actively developed.  The SST Security Toolkit (SST) was a project at opensolaris.org.  That repo has been removed, so I uploaded SST to GitHub for anyone who might have a historical interest in the product.  For Solaris 11 security auditing, refer the OpenSCAP documentation.

OpenSCAP does not implement security controls.  The SCAP spec for implementation is still in draft, and will likely take some time to mature.  There's a clear need for a project like this, and I'd still like to persue the [goals](https://blogs.oracle.com/sst/entry/minutes_from_4_june_2010) outlined by the legacy opensolaris.org SST blog.  Please [email me](mailto:jason@jasoncallaway.com) if you're interested in contributing.

Thanks,

~Jason


Legacy SST Project Page...

#SST Security Toolkit

##What is SST?

The SST Security Toolkit (SST) is a flexible Unix and Linux hardening tool.  SST simplifies and automates the hardening process which allows administrators to apply security settings consistently across the enterprise.

SST was formerly known as the Solaris Security Toolkit and as and the JumpStart Architecture and Security Scripts (JASS) Toolkit.

##SST Branches

One of the core goals of the open source SST project is platform independence.  However, since SST has a loyal following among Solaris administrators the project will maintain two branches – one for legacy Solaris support, another for platform independent *nix support.

###SST Security Toolkit: Community Edition (SST:CE)

The Community Edition (or just ‘CE’) will support OpenSolaris, Solaris 10, Red Hat Enterprise Linux (RHEL), and any other operating system in which the community has interest.  In addition to platform independent support, CE will focus on security standards like SCAP and CVE.

###SST Security Toolkit: Legacy Version (SST:LV)

The Legacy Version (or just ‘LV’) is all about continuity.  It is an evolutionary release for SST 4.2 that will support Solaris 10 SPARC and x86/x64. Anyone familiar with SST 4.2 will find transitioning to LV to be easy if not seamless.  LV development work will be mostly backwards-compatibility, updated drivers, and .fin and .aud scripts to support the security standards like SCAP.

The latest SST:LV - SUNWjass 4.2.2

Download the latest version of SST:LV - SUNWjass 4.2.2.  This is a beta version, so use caution when executing against mission systems.

Where to find SUNWjass 4.2

If you're looking for the older Solaris Security Toolkit version 4.2, you can find it at http://www.sun.com/software/security/jass/.

##Development Goals

If you're wondering about what SST means to accomplish, check the Goals and Use Cases pages.
Getting Started

Want to contribute to SST?  Here's how.

    Grab the SST:CE source tree

    hg clone ssh://hg.opensolaris.org/hg/sst/sst-ce

    Or if you're interested in SST:LV, you can grab that source tree here:

    hg clone ssh://hg.opensolaris.org/hg/sst/sst-lv

        To build: `cd src; make all; make pkgdefs`.  Your new package will be in src/Releases.
    Then check out the To do list, grab an action and dive in.
    When you're done, email security-discuss to discuss committing your changes.

If you're new to OpenSolaris or Mecurial there's a great how-to page here.
The SST Blog

Keep up to date with the SST blog: http://blogs.oracle.com/sst.  You can find nifty things there like meeting minutes and conference call recordings.

Send an email to jason dot callaway at oracle dot com if you have comments or questions.

