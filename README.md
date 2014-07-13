cydia-repo.tihmstar.org
==========

This repo is not meant to be clone by regular user. If you want to get it's content you should add "repo.tihmstar.org" and download the tool via Cydia or apt.

This is a cydia undeb-repo demo. If you want to maintain your package hosted on my repo, you need to (asking tihmstar first) make such an undeb-repo on your git. There you can push your changes and my daemon will clone your git repo, build a deb and push to my Cydia repo.

You need to create a new repo in your git which must be named "cydia-repo.tihmstar.org"
In the README.md I advise you to copy the first part from this file.

Create a folder for each package you want to sumbit and name it with the package ID. Inside this package directory put the files the package contains.

You must have a `packageID/DEBIAN/control` file which must at least contain:

* "Package" (id of your package)
* "Name" (name displayed in cydia)
* "Version" (your package version)
* "Author" (your name)

Check any control files in this repository to see how to format said file.
