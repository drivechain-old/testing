Testing Drivechains
===================

Setup
-----

### Mainchain (bitcoin) setup
- Download (clone)
'''
git clone https://github.com/drivechain-project/mainchain.git
'''

- Build
'''
./autogen.sh
./configure (optional: --with-incompatible-bdb --disable-tests)
make
'''

- Data directory
You will need to create a new data directory to store the blockchain, DB etc
for bitcoin (mainchain). In this example a new directory 'drivechainMain' will
be created in your home directory.
'''
mkdir ~/drivechainMain
'''

- Configuration file
Copy the main.conf configuration file from
[Drivechain testing repository](https://github.com/drivechain-project/testing)
to ~/drivechainMain/bitcoin.conf

### Sidechain setup
- Download (clone)
'''
git clone https://github.com/drivechain-project/sidechain.git
'''

- Build
'''
./autogen.sh
./configure (optional: --with-incompatible-bdb --disable-tests)
make
'''

- Data directory
You will need to create a new data directory to store the blockchain, DB etc
for the sidechain. In this example a new directory 'drivechainSide ' will be
created in your home directory.
'''
mkdir ~/drivechainSide
'''

- Configuration file
Copy the side.conf configuration file from
[Drivechain testing repository](https://github.com/drivechain-project/testing)
to ~/drivechainSide/bitcoin.conf

Testing (manual)
----------------


Testing (automated) TODO
------------------------
