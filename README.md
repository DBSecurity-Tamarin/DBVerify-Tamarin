# DBSecurity-Tamarin

## Introduction

This repository contains the source files for Tamarin analysis of distance-
bounding security protocols.

The website for the Tamarin prover tool is located at [http://tamarin-prover.github.io/](http://tamarin-prover.github.io/).

## Folder Layout

tamarinprotocols/ contains the .spthy files used by Tamarin for the analysis.
If the Tamarin tool is installed on your device, they can be executed by the command
```tamarin-prover --prove <filename>```

mscs/ contains pdf diagrams showing the intended
execution trace of each protocol. These diagrams are slightly abstracted
from the original definition of the protocol - in most cases, this is
the conversion of the fast phase of a communication protocol from a series
of short messages to one long message. At times, the equational theory
has been changed to a strictly stronger version than that provided in the
original paper. The existence of an attack on the abstracted protocol
indicates the existence of an attack on the original version.