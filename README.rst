sphinxjp.tk0miya
=============================

This is a sphinx extension which inserts a flickr photo on your
document.

Setting
=======

Install
-------

::

   $ pip install sphinxjp.tk0miya


Configure Sphinx
----------------

To enable this extension, add ``sphinxjp.tk0miya`` module to extensions
option in `conf.py`.

::

   # Enabled extensions
   extensions = ['sphinxjp.tk0miya']

You should get access token from Flickr and set filckr_api_key and flickr_secret in
your conf.py

::

   flickr_api_key="<YOUR_API_KEY_PUT_HERE>"
   flickr_secret="<YOUR_SECRET_PUT_HERE>"


usage
=====================

::

   .. flickr-search:: marriage

random
------------

flickr-search put only a first image. You can set `:random:` as option
to put a randomized image.

::

   .. flickr-search:: marriage
      :random:

license
--------

You can set search license by setting license option.

::

   .. flickr-search:: marriage
      :license: 0,1

possible values are

- 0 All Rights Reserved
- 1 `Attribution-NonCommercial-ShareAlike License <http://creativecommons.org/licenses/by-nc-sa/2.0/>`_
- 2 `Attribution-NonCommercial License <http://creativecommons.org/licenses/by-nc/2.0/>`_
- 3 `Attribution-NonCommercial-NoDerivs License <http://creativecommons.org/licenses/by-nc-nd/2.0/>`_
- 4 `Attribution License <http://creativecommons.org/licenses/by/2.0/>`_
- 5 `Attribution-ShareAlike License <http://creativecommons.org/licenses/by-sa/2.0/>`_
- 6 `Attribution-NoDerivs License <http://creativecommons.org/licenses/by-nd/2.0/>`_
- 7 `No known copyright restrictions <http://flickr.com/commons/usage/>`_
- 8 `United States Government Work <http://www.usa.gov/copyright.shtml>`_

If you want to search multiple licenses, use comma-separated.

size
--------

::

   .. flickr-search:: marriage
      :size: Small

Possible values are

- "square"
- "large Square"  # note: Square is Uppwer case but large is Lower
- "thumbnail"
- "small"
- "small 320"
- "medium"
- "medium 640"
- "medium 800"
- "large"
- "original"


Repository
==========

https://bitbucket.org/r_rudi/sphinxjp.tk0miya


License
========

The BSD 2-Clause License.

Note
===============

This extention is created for marriage of "World `tk0miya
<https://twitter.com/tk0miya>`_ ". Congratulations on your wedding!
