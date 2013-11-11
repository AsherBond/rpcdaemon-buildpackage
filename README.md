RPC Daemon (Havana work in progress)
==========

**THIS IS AN ACTIVE WORK IN PROGRESS**
*It is probably unusable at any given time.*

This is an AMQP RPC Daemon, primarily intended for tracking and responding to OpenStack Neutron agent state changes and rescheduling resources appropriately.

It currently supports L3 agents, DHCP agents and a special Dump plugin to blindly log RPC messages.

The current framework correctly daemonizes and operates as a singleton by using a pidfile.

## License ##

All files licensed under the Apache-2 license (see LICENSE), with the
exception of `rpcdaemon/lib/limits.py` and `rcpdaemon/lib/mixin.py`, which
are pulled from Kombu 1.4.0, and have the following license:


    Copyright (c) 2012-2013 GoPivotal, Inc.  All rights reserved.
    Copyright (c) 2009-2012, Ask Solem & contributors.
    All rights reserved.

    Redistribution and use in source and binary forms, with or without
    modification, are permitted provided that the following conditions are met:

        * Redistributions of source code must retain the above copyright
          notice, this list of conditions and the following disclaimer.
        * Redistributions in binary form must reproduce the above copyright
          notice, this list of conditions and the following disclaimer in the
          documentation and/or other materials provided with the distribution.
        * Neither the name of Ask Solem nor the
          names of its contributors may be used to endorse or promote products
          derived from this software without specific prior written permission.

    THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
    AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
    THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
    PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL Ask Solem OR CONTRIBUTORS
    BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
    CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
    SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
    INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
    CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
    ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
    POSSIBILITY OF SUCH DAMAGE.
