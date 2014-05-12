======
Scrapy
======

.. image:: https://badge.fury.io/py/Scrapy.png
   :target: http://badge.fury.io/py/Scrapy

.. image:: https://secure.travis-ci.org/scrapy/scrapy.png?branch=master
   :target: http://travis-ci.org/scrapy/scrapy

Overview
========

Scrapy is a fast high-level screen scraping and web crawling framework, used to
crawl websites and extract structured data from their pages. It can be used for
a wide range of purposes, from data mining to monitoring and automated testing.

For more information including a list of features check the Scrapy homepage at:
http://scrapy.org

Requirements
============

* Python 2.7
* Works on Linux, Windows, Mac OSX, BSD

Install
=======

The quick way::

    pip install scrapy

For more details see the install section in the documentation:
http://doc.scrapy.org/en/latest/intro/install.html

Releases

在windows下安装真是蛋疼，首先的问题是lxml的安装，他会提示一个错误：“unable to find vcvarsall.dll”.
你得设置VS90COMNTOOLS这个环境变量，设为相应的VC环境即可，我的是VS2010的环境，所以它的值为“C:\Program Files\Microsoft Visual Studio 10.0\Common7\Tools\”。
ok，再使用pip install lxml的时候不会有该错误了，但是出现了另外一个错误：是说lxml的头文件没有找到，所以得自己安装lxml。
然后使用easy_install lxml居然成功了，受不了...
然后继续使用pip安装，没有问题...
然后再命令行下使用scrapy的时候出现了一个问题“dll load failed”.这说明openssl没有装好，一般来说装好openssl之后得重启，
所以我重启了，果然下次这个命令就行了，但是又突然发现TMD校园网连不上了！提示定位不到libeay32.dll，真是操蛋，没办法，
重装校园网。还好，新的校园网认证客户端有自己的libeay32.dll这个库。这样总算是装成功了！
========

You can download the latest stable and development releases from:
http://scrapy.org/download/

Documentation
=============

Documentation is available online at http://doc.scrapy.org/ and in the ``docs``
directory.

Community (blog, twitter, mail list, IRC)
=========================================

See http://scrapy.org/community/

Contributing
============

See http://doc.scrapy.org/en/latest/contributing.html

Companies using Scrapy
======================

See http://scrapy.org/companies/

Commercial Support
==================

See http://scrapy.org/support/
