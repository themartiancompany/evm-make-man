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


=================================
evm-contract-deployments-dir
=================================

------------------------------------------------------------------------------
Ethereum Virtual Machine (EVM) contract deployments directory discovery tool
------------------------------------------------------------------------------
:Version: evm-contract-deployments-dir |version|
:Manual section: 1

Synopsis
========

evm-contract-deployments-dir *[options]* *app-name*

Description
===========

Returns default deployments directory for an application




Options
=======

-u, --user-level        Returns user-level location for
                        an application deployments.
                        Defaults to 'n'.

-h                      Displays help.
-c                      Enable color output
-v                      Enable verbose output

Bugs
====

https://github.com/themartiancompany/evm-contracts-tools/-/issues

Copyright
=========

Copyright Pellegrino Prevete. AGPL-3.0.

See also
========

* evm-contract-call
* evm-contract-deployment-address
* evm-contract-deployments-dir
* evm-contract-deployment-networks
* evm-contract-deployment-versions
* evm-contracts-abi-get
* evm-wallet

.. include:: variables.rst
