Google/Yandex search link fix
=============================

Google/Yandex search link fix is a Firefox extension that prevents Google and Yandex search pages from modifying search result links when you click them. This is useful when copying links but it also helps privacy by preventing the search engines from recording your clicks. [Detailed description](https://palant.de/2011/11/28/google-yandex-search-link-fix)

Prerequisites
-------------
* [Python 2.7](https://www.python.org/downloads/)
* [Jinja2 module for Python](http://jinja.pocoo.org/docs/intro/#installation)
* Adblock Plus build tools (clone https://github.com/adblockplus/buildtools.git into the `buildtools` subdirectory)

How to build
------------

Run the following command:

    python build.py build

This will create a development build with the file name like `searchlinkfix-1.2.3.nnnn.xpi`. In order to create a release build use the following command:

    python build.py build --release

How to test
-----------

Testing your changes is easiest if you install the [Extension Auto-Installer extension](https://addons.mozilla.org/addon/autoinstaller/). Then you can push the current repository state to your browser using the following command:

    python build.py autoinstall 8888

Google/Yandex search link fix will be updated automatically, without any prompts or browser restarts.