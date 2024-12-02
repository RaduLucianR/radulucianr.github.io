---
title: "16-bit Brent-Kung Adder"
excerpt: "<img src='/images/portfolio/thumbnails/adder.png'>"
collection: portfolio
date: 19-January-2023
---
**Project attribution**: Project done nearly solo with help from Ahmed Ghanem and Eric Abraham. <br>
**Source**: The project's files are available [here](https://github.com/RaduLucianR/adder). <br>
**Short description**: 16-bit Brent-Kund Adder Digital IC Design <br>
**Technologies**: Cadence Virtuoso <br>
**What I did**: I designed and implemented the schematic and layout of (nearly all) components and of the entire adder.

This is a schematic and layout of an IC design that implements a 16-bit full adder following [the Brent-Kung architecture](https://en.wikipedia.org/wiki/Brent%E2%80%93Kung_adder). The schematic and layout were made for $$45nm$$ CMOS technology, using the industry standard [Cadence Virtuoso software](https://www.cadence.com/en_US/home/tools/custom-ic-analog-rf-design/layout-design/virtuoso-layout-suite.html).

The adder layout has a total surface of $$177 um^2$$ and a maximum critical path delay of $$200 ps$$. The layout design leverages custom odd/even black/grey cells and custom preprocessing cells that don't use other gates underneath. This allows us to reduce the area of their layouts, and consequently the area of the entire adder. You can checkout the schematics and layouts of all components in the [`images` folder](https://github.com/RaduLucianR/adder/tree/main/images) of the Github repository.

### Adder
<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/adder/adderSchematic.png' style="display: block; margin-left: auto; margin-right: auto; width:95%">
    <figcaption>Full schematic of the adder. The square symbols represent black cells, while the diamond symbols represent grey cells. Each black/grey cell is marked with an O/E to highlight whether they are odd or even, respectively.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/adder/adderLayout.png' style="display: block; margin-left: auto; margin-right: auto; width:95%">
    <figcaption>Full layout of the adder.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/adder/adderTest.png' style="display: block; margin-left: auto; margin-right: auto; width:95%">
    <figcaption>Test setup of the adder. We use random bit generators to generate 2 random 16-bit numbers and a carry. Each square component is a random bit generator. The component marked with Z is the adder. Then, we inspect the voltages in the output 16-bit bus and assert whether they are correct. The assertion is done using the Calculator tool of Cadence Virtuoso.</figcaption>
</figure>

<figure style="flex-direction: column; align-items: center; justify-content: center; text-align: center;">
    <img src='/images/portfolio/adder/lvs.png' style="display: block; margin-left: auto; margin-right: auto; width:60%">
    <figcaption>Positive result of the Layout Versus Schematic (LVS). This confirms that the layout and schematic are equivalent. Moreover, this also confirms that the Design Rule Checking (DRC) analysis passes as well, i.e. there are no violations of the layout design rules.</figcaption>
</figure>

