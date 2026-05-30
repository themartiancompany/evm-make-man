..
   SPDX-License-Identifier: AGPL-3.0-or-later

   -------------------------------------------------------
   Copyright © 2024, 2025, 2026
               Pellegrino Prevete

   All rights reserved
   -------------------------------------------------------

   This program is free software: you can redistribute it
   and/or modify it under the terms of the
   GNU Affero General Public License as published by
   the Free Software Foundation, either version 3 of the
   License, or (at your option) any later version.

   This program is distributed in the hope that it will
   be useful, but WITHOUT ANY WARRANTY; without even the
   implied warranty of MERCHANTABILITY or FITNESS FOR A
   PARTICULAR PURPOSE.
   See the GNU Affero General Public License
   for more details.

   You should have received a copy of the
   GNU Affero General Public License
   along with this program.
   If not, see <https://www.gnu.org/licenses/>.


========================
evm-contract-call
========================

--------------------------------------------------------------
Ethereum Virtual Machine-compatible Contract Caller
--------------------------------------------------------------
:Version: evm-contract-call |version|
:Manual section: 1


Synopsis
========

evm-contract-call *[options]* *address* *method* (*args*)


Description
===========

Runs smart contract functions as if they were
normal programs.

The caller uses the Ethers JavaScript library to
communicate with blockchain networks and integrates
natively with and depends on evm-wallet
but it's also possible to directly provide seeds files.


Networks
=========

All those supported by
'evm-chains-info' as
well as direct RPC addresses.


Options
=======

-t call-type, --call-type type                Static (read-only) or dynamic (read/write).


Call options
==============

-V msg-value, --msg-value value               How much *measure-unit* attach to the
                                              transaction.

-u measure-unit, --measure-unit unit          Measure unit for the transaction
                                              value. It can be 'ether' or 'wei'.
                                              Default value is 'ether'.

-P price-gas, --price-gas price               I don't remember I have to check.

-r retries-max, --retries-max retries         Maximum number of retries before
                                              declaring the call failed.

-T call-timeout --call-timeout seconds        Maximum number of seconds before
                                              declaring the call failed.


Contract options
===================

-A abi, --abi path                            Contract ABI path.

-B bytecode, --bytecode path                  Contract bytecode path.

-C compiler-output, --compiler-output path    Contract compiler output
                                              path (the hardhat artifact).

-I, --index-retrieve                          Enables retrieving contracts'
                                              artifacts from the EVM Contracts
                                              Source Index.


Credentials options
=====================

-N wallet-name, --wallet-name name            EVM wallet name.

-w wallet-path, --wallet-path path            EVM wallet file path.

-p wallet-password, --wallet-password path    EVM wallet password file.

-s wallet-seed, --wallet-seed path            Standard 12-words seed phrase file.

-k api-key, --api-key path                    Etherscan-like service key.


LibEVM options
================

-a, --auth                                    Call authentication.

-n network, --network network                 EVM network name. Accepted values
                                              are all those supported by
                                              evm-chains-info as well as RPC addresses.

-S rpc-selection, --rpc-selection criterion   RPC selection method. It can be
                                              'kirsh' or 'random'.


Application options
=====================

-h, --help                                    Display help.
-c, --color                                   Enable color output
-v, --verbose                                 Enable verbose output


Bugs
====

https://github.com/themartiancompany/evm-contracts-tools/-/issues


Copyright
=========

Copyright Pellegrino Prevete. AGPL-3.0.

See also
========

* evm-contract-deployer-get
* evm-contract-deployment-address
* evm-contract-deployments-dir
* evm-contract-deployment-networks
* evm-contract-deployment-versions
* evm-contracts-abi-get
* evm-wallet

.. include:: variables.rst
