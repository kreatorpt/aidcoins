Aidcoins integration/staging tree
================================

http://aidcoins.org

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2011-2014 Litecoin Developers
Copyright (c) 2014-2014 Aidcoins Developers

What are Aidcoins?
----------------

THE SOCIAL DIGITAL COINS

Aidcoins is based on Aidcoins, but inovates in the social sector, we like to help
end poberty on the World!

This ideia born in Portugal em 2014, a contry in economic crisis. This lead to ideias that can help the World to 
be a better place!

Any coin transfer require a minimum of 2% donation for a registed social 
solidarity institution anyhere in the World, the "list" of those institutions are public 
avaible at http://aidcoins.org/list this is the only central managed part of the Aidcoin.

The "list" have 3 field, world location (location), institution name (name) and wallet address (address).

Record example: "Europe/Portugal", "AMI Portugal", "232jdasfas234*************"

The wallet will made updates of that list every day, if the server is offline, the list 
remains unchanged.

Any donation will only be validated if the destination address is on the "list".
Any coin transfer betten users will only be validated, if follows a donation tranfer of at least 2% of the value 
to transfer to a normal user wallet.

This coin is to be used by conscienced people! 
Poberty proves that Humans failed as a society!


Aidcoins is using scrypt as a proof-of-work algorithm.
 - 2.5 minute block targets
 - subsidy halves in 840k blocks (~4 years)
 - ~84 million total coins

The rest is the same as Aidcoins and Bitcoin.
 - 200 coins per block
 - 2016 blocks to retarget difficulty

For more information, as well as an immediately useable, binary version of
the Aidcoin client sofware, see http://www.todo-later.org.

License
-------

Aidcoins is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process ##### rever daqui para baixo.
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Aidcoins
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion (if they haven't already) on the
[mailing list](http://sourceforge.net/mailarchive/forum.php?forum_name=bitcoin-development).

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/bitcoin/bitcoin/tags) are created
regularly to indicate new official, stable release versions of Aidcoins.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./aidcoins-qt_test

