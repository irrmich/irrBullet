[![Build Status](https://travis-ci.org/Artistic-Games/DIrrlicht.png?branch=master)](https://travis-ci.org/Artistic-Games/irrBullet)
[![Stories in Ready](https://badge.waffle.io/Artistic-Games/irrBullet.png?label=ready&title=Ready)](https://waffle.io/Artistic-Games/irrBullet)

irrBullet - Bullet Physics Wrapper for Irrlicht Engine
======================================================

Details
-------

This is a fork of irrBullet, which can be found at https://irrbullet.svn.sourceforge.net/

It is an updated version of irrBullet which works with Irrlicht 1.8.1 and latest SVN branch (unstable) and Bullet 2.83. It also has several improvements over outdated irrBullet. I tried contacting the original author of irrBullet, but got no response.

Note: The following version hasn't released yet and maybe unstable. If you find any bug, then please open an issue in issues tracker. Thanks.

What's new in 0.1.9
-------------------
* Performance improvement (refactored loops, replaced Irrlicht's containers with STL, add move semantics etc)
* Several bug fixes
* Support for latest versions of Bullet and Irrlicht
* ICapsuleShape and ICylinderShape added
* IRigidBody, irrBulletWorld etc are feature complete (all methods have been wrapped)
* Strong C++11 support - dropped support for non-C++11 compilers
* irrBullet is forked - now maintained by Danyal Zia

Installation
------------

On windows open Dependencies_Path.bat in directory and change respective environment variables to Bullet and Irrlicht's root directory and run it, then in "source/" open the project file of your favorite IDE (Visual Studio and Code::Blocks is currently supported) and compile. You will then find the compiled library in "lib/your_platform".

To compile examples go to "examples/" and open the project and compile, you'll then find the compiled binaries in "bin/your_platform". Please note that if you have compiled using shared Irrlicht binary then you need to copy Irrlicht.dll/.so from Irrlicht's directory to "bin/your_platform" in order to run the examples.

License
-------

It is released under permissive zlib license same as Bullet and Irrlicht.
