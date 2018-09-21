
<a href="https://imgbb.com/"><img src="https://image.ibb.co/czB4ge/Lightningcash_logo.png" alt="Lightningcash_logo" border="0"></a>





Lightningcash Core integration/staging tree
=====================================

[![Build Status](https://travis-ci.org/MerlinMagic2018/lightningcash.svg?branch=master)](https://travis-ci.org/MerlinMagic2018/lightningcash)

Official Website :

http://lightningcash.cf/

( still need to be updated )


Official stratum pool website :

http://lightningcash.tk:8080/

Official Block Explorer :

http://lightningcash-explorer.tk:3001/




Exchanges listing to be announced in the future. Important dates and information will be available on the official website.


Looking for serious long-term developpers to :

-- integrate a multi-exchange platform right in the wallet GUI, through available exchanges APIs.


Releases : 

Windows 64bits wallet installer : https://ufile.io/i02r1

Linux lightningcash.conf file : https://ufile.io/3p9iu 
( must be placed in /home/username/.lightningcash/lightningcash.conf )

Official node : 18.224.50.0:9191



Build instructions
----------------

See /doc/build-unix.md
or /doc/build-windows.md

What is Lightningcash?
----------------

Lightningcash is an experimental digital currency that aims to enables instant payments to
anyone, anywhere in the world. That will hopefully become true if it is eventually widly accepted and listed on exchanges. ;-) 

Lightningcash uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. Lightningcash Core is the name of open source
software which enables the use of this currency.

Information and an immediately useable, binary version of
the Lightningcash Core GUI binary releases are available. See Binary Releases.

License
-------

Lightningcash Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/MerlinMagic2018/lightningcash/tags) will be created
regularly to indicate new official, stable release versions of Lightningcash Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).



Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).

There are also [regression and integration tests](/test), written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/test) are installed) with: `test/functional/test_runner.py`

The Travis CI system makes sure that every pull request is built for Windows, Linux, and OS X, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

We only accept translation fixes that are submitted through [Bitcoin Core's Transifex page](https://www.transifex.com/projects/p/bitcoin/).
Translations are converted to Lightningcash periodically.

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.
