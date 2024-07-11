---
title: "Retransmission Protocol"
excerpt: "<img src='/images/portfolio/thumbnails/caal.png'>"
collection: portfolio
date: 04-June-2021
---
Project done in collaboration with Yip van Ginkel.

Design of a communication protocol called "Retransmission Protocol" using CCS (Calculus of Communicating Systems) and verification using HML (Hennesy-Milner Logic). Check the Context section at the bottom of the page for more information. Implementation done using the [CAAL](https://caal.cs.aau.dk/) tool.

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/caal/caal_ccs.png' style="display: block; margin-left: auto; margin-right: auto; width:100%">
    <figcaption>GUI of the editor pane of CAAL. Our CCS code can be seen in the central panel.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/caal/hml_rules.png' style="display: block; margin-left: auto; margin-right: auto; width:50%">
    <figcaption>HML rules for deadlock and livelock.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/caal/caal_hml.png' style="display: block; margin-left: auto; margin-right: auto; width:100%">
    <figcaption>GUI of the verification pane of CAAL. Some of our HML rules and their verification results can be seen in the central panel.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/caal/deadlock.png' style="display: block; margin-left: auto; margin-right: auto; width:70%">
    <figcaption>Verification results for the deadlock rule. The verification rules are true if a state of the system is found for which the verification rule holds. Since no state was found where the deadlock rule holds, then the result is false, hence there is no deadlock. There are 4 types of communication channels that were tested: reliable, noisy, lossy, lossy and duplicative.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/caal/livelock.png' style="display: block; margin-left: auto; margin-right: auto; width:70%">
    <figcaption>Verification results for the livelock rule. There are live locks found for the unreliable channels which could be attributed to the fact that these channles can lose messages ad infinitum, while the reliable communication channel does not.</figcaption>
</figure>

### Context
The goal is to model and analyse a communication protocol that is tolerant for communication through a medium that is not com-
pletely reliable (e.g., because it may so now and then lose or compromise messages). If some company proposes the protocol described informally below we might be hired by them to use formal modelling and analysis techniques to confirm the correctness of their proposal. Below
you will find their informal description of the protocol in plain English. The main goal is not to improve the protocol as described below. The goal is rather to report to the company to what extent their proposal is correct. (If the report contains potential 
flaws in the protocol, then we are able to defend to the company why our modelling is according to their description.)

The protocol describes the behaviour at the side of the sending party (say S) and at the side
of the receiving party (say R). The protocol's task is to take care of managing the retransmission
of messages that arrive corrupted or are lost by this next lower layer, so that the messages that
are sent through S arrive correctly and in-order at R. RP achieves this as follows:
* Each message sent by S is extended with an additional control bit, l(ow) or h(igh).
* When S sends a message, it does so repeatedly (each time sending along its corresponding
bit) until it receives an acknowledgment from R that contains the same bit as the message
being sent.
* When R receives a message, it sends an acknowledgment to S and includes the bit of the
received message. Moreover, when a message is received for the first time, the receiver
delivers it (to the receiving entity) for processing, while subsequent messages with the bit
are simply acknowledged.

When S receives an acknowledgment containing the same bit as the message it is currently
transmitting, it stops transmitting that message, toggles the bit and repeats the protocol for the
next message.