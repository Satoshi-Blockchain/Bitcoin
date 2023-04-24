Blockchain Core integration/staging tree
=====================================

https://blockchaincore.net

For an immediately usable, binary version of the Blockchain Core software, see
https://blockchaincore.net/en/download/.

What is Blockchain Core?
---------------------

Blockchain Core connects to the Bitcoin peer-to-peer network to download and fully
validate blocks and transactions. It also includes a wallet and graphical user
interface, which can be optionally built.

Further information about Blockchain Core is available in the [doc folder](/doc).

License
-------

Blochcain Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built (see `doc/build-*.md` for instructions) and tested, but it is not guaranteed to be
completely stable. [Tags](https://github.com/bitcoin/bitcoin/tags) are created
regularly from release branches to indicate new official, stable release versions of Blockchain Core.

The https://github.com/blockchain-core/gui repository is used exclusively for the
development of the GUI. Its master branch is identical in all monotree
repositories. Release branches and tags do not exist, so please do not fork
that repository unless it is for development reasons.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md)
and useful hints for developers can be found in [doc/developer-notes.md](doc/developer-notes.md).

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
in Python.
These tests can be run (if the [test dependencies](/test) are installed) with: `test/functional/test_runner.py`

The CI (Continuous Integration) systems make sure that every pull request is built for Windows, Linux, and macOS,
and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

Changes to translations as well as new translations can be submitted to
[Bitcoin Core's Transifex page](https://www.transifex.com/bitcoin/bitcoin/).

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.

Copyrights Information: Blockchain core first implementation is tested on Bitcoin Project by 
Satoshi Nakamoto, which is known as Bitcoin Network and the Software Client name is Bitcoin Core.
The building block of Bitcoin Core is the Blockchain technology that uses Cryptographic protocol 
SHA-256 to develop on chain hash to crate the Bitcoin Blockchain.

Bitcoin and Blockchain copyrights are protected by its inventor and it was first released under 
the MIT Open Source Licene. 

Forking: Forking of Bitcoin Blockchain is not permitted but any one can clone the Code and create 
Altcoin, which Satoshi Nakamoto permitted. Forking Bitcoin Blockchain is a violation, and it can 
lead to a legal dispute, which can proceed to a corporate litigation.  Therefore, it is advised to 
respect the inventors Copyrights and Cloning Forking Protocols.

Integration of Bitcoin and Bitcoin Core in Blockchain Core is upgraded by its inventor and owner,
Satoshi Nakamoto. 


