# Rubicon: Precise Microarchitectural Attacks with Page-Granular Massaging

Welcome to the Rubicon repository! Rubicon is the first deterministic, general-purpose memory massaging primitive for microarchitectural attacks. It enables precise and reliable control over where data lands in physical memory, something that attacks like Rowhammer and Spectre fundamentally depend on. By manipulating the state of the Linux allocator, Rubicon replaces fragile techniques like spraying and brute-force scanning with a fast, robust, and scalable solution. This opens the door to practical, high-reliability exploitation that was previously infeasible.

This repository provides all the resources necessary to explore, reproduce, and build upon our work. For more details about Rubicon, please visit our [website](https://comsec.ethz.ch/rubicon/) or read our [research paper](https://comsec.ethz.ch/wp-content/files/rubicon_eurosp25.pdf).

## Repository Overview
- **rubicon-mechanisms**: Implements the core Rubicon mechanisms, designed to manipulate the Linux memory allocator for deterministic control over physical memory placement.
- **rubicon-microbenchmarks**: Contains microbenchmarks used to evaluate the performance and effectiveness of the Rubicon mechanisms.
- **rubicon-blacksmith**: Extends the Blacksmith Rowhammer fuzzer with Rubicon, creating a complete end-to-end Rowhammer attack.
- **rubicon-retbleed**: Features the Rubicon-enhanced Retbleed attack, which precisely positions `/etc/shadow` at a known physical memory location, eliminating the need for the original Retbleed's lengthy scanning phase.

We hope Rubicon serves as a valuable resource for your research and development efforts. Contributions and feedback are always welcome!

## Citing our Work
To cite Rubicon in academic papers, please use the following BibTeX entry:

```
@inproceedings{boelcskei_rubicon_2025,
	title = {{Rubicon: Precise Microarchitectural Attacks with Page-Granular Massaging}}, 
	url = {Paper=https://comsec.ethz.ch/wp-content/files/rubicon_eurosp25.pdf},
	booktitle = {{EuroS\&P}},
	author = {Bölcskei, Matej and Jattke, Patrick and Wikner, Johannes and Razavi, Kaveh},
	month = jun,
	year = {2025},
	keywords = {dir\_os, type\_conf}
}
```