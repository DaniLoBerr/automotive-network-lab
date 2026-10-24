# automotive-network-lab

A small lab to practise testing automotive network software:

- a simulated ECU that offers a SOME/IP service over UDP, written in Python, C and C++;
- one pytest suite that validates all three, with a JUnit report and Wireshark captures as evidence;
- a simulated CAN rest-bus, with a test for message periods;
- and CI that runs everything on every change.

Work in progress: built ticket by ticket, through the issues and pull requests of this repo.
