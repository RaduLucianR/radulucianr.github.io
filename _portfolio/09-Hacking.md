---
title: "Man-in-the-middle attacks"
excerpt: "<img src='/images/portfolio/thumbnails/hacking.png'>"
collection: portfolio
date: 30-June-2021
---
**Project attribution**: Project done in collaboration with Teodor Lungu. <br>
**Source**: The project's source code is available [here](https://github.com/RaduLucianR/2IC80_HackingProject). <br>
**Short description**: Python app that executes standard man-in-the-middle attacks: ARP table poisoning, DNS spoofing and TCP Telnet session hijackin. <br>
**Technologies**: Python, [Tkinter](https://docs.python.org/3/library/tkinter.html), [Scapy](https://scapy.net/).<br>
**What I did**: I implemented the GUI and the ARP and DNS attacks, but also helped around with polishing the TCP hijacking.

We designed and implemented a lightweight tool in Python using the Scapy network packets manipulation library, for 3 network attacks: [ARP table poisoning](https://en.wikipedia.org/wiki/ARP_spoofing), [DNS spoofing](https://en.wikipedia.org/wiki/DNS_spoofing) and [TCP Telnet session hijacking](https://www.usna.edu/Users/cs/choi/it432/lec/l04/lec.html). I also implemented a GUI with the Tkinter library for ease of use.

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/hacking/hostsTab.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>First panel. It displays the available hosts in a list.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/hacking/arpPoisoned.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>ARP Poisoning panel after successful poisoning.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/hacking/dnsSpoofed.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>DNS Spoofing panel after successful spoofing.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/hacking/mitmError.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>Error handling for DNS spoofing when the user did not execute ARP table poisoning beforehand to become MITM.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/hacking/tcpTab.png' style="display: block; margin-left: auto; margin-right: auto; width:80%">
    <figcaption>TCP session hijacking panel before initiating the attack.</figcaption>
</figure>