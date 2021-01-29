# FAQs

## General FAQs

### What is Haiku?

Haiku is a fast, efficient, easy to use and lean open source operating system inspired by the BeOS that specifically targets personal computing. It is also the name of the project that develops and promotes Haiku the operating system.

### Is Haiku based on Linux?

Haiku is not a Linux distribution, nor does it use the Linux kernel.  Linux-based distributions stack up software – the Linux kernel, the X Window System, and various DEs with disparate toolkits such as GTK+ and Qt – that do not necessarily share the same guidelines and/or goals.  Haiku has a single focus on personal computing and is driven by a unified vision for the whole OS.

### What platform(s) is Haiku targeted to run on?

The main target for Haiku R1 is the x86 (Intel, AMD, and compatible) platform. There are [ports to other platforms underway](https://www.haiku-os.org/guides/building/port_status) (external link), such as PowerPC, Sparc, and ARM. However, it is not clear whether these will be supported or not. It will heavily depend on the availability of resources to support their development.

### What are the minimum hardware requirements to run Haiku?

The x86 32-bit release of Haiku will run on a Pentium or better CPU with 256 MiB of RAM (as long as virtual memory is activated), 1.5 GiB of storage space and a VESA compliant video card.

However, for a satisfactory user experience, we recommend **at least** a Pentium4 with 512 MiB of RAM and 2 GiB of storage space. For compiling Haiku within itself, 2 GiB of RAM is recommended.

### What license is Haiku released under?

Most of the Haiku code is released under the very liberal [MIT License](https://opensource.org/licenses/mit-license.php). Some third party components (e.g.: some media codecs, libraries, etc.) may use other licenses.  The Haiku source tree has very few ported applications, and with the advent of package management, even these are being migrated out of the tree. For most applications it is preferable that their Haiku port is maintained in the original vendor's source repository. Third party libraries are usually only included when they are used by components (applications, libraries) we consider essential. Kernel drivers for hardware support, on the other hand, are almost always welcome.  ([https://www.haiku-os.org/development/faq#acceptable-licenses](https://www.haiku-os.org/development/faq#acceptable-licenses))

### Is there a 64-bit version of Haiku?

Yes. For R1 we are targeting two architectures, 32-bit x86 (i586 and newer) and 64-bit x86_64.  Regarding GCC, we use GCC 8 for most things (i.e. 64-bit and most of the 32-bit OS), while GCC2 is used for BeOS compatibility.

The 32-bit release is compatible with the BeOS at a binary and API level (hybrid GCC2 / GCC 8). The 32-bit Haiku release can run most BeOS applications without modification or recompiling.

The 64-bit release is not binary compatible with BeOS (GCC 8), but still enjoys compatibility with the powerful BeOS API.

### What is the goal of Haiku?

Our main selling point is good support for modern hardware, a stable OS, already a reasonable number of apps available, a well-polished user interface, a lightweight system.  Having the whole OS in a single place makes it easy to do some experiments where you just change the code and see what happens.  The end goal of Haiku is having an OS with its own, well integrated, native applications.

- **Early adopters**
- **Academic research**
- **Open source programming**
- **Desktop user looking for fast, responsive system**

## **Developer FAQ’s**

### I am a programmer and would like to help. Where can I get started?

Check out the *Getting Started* page. You will also find links to several useful development related pages in the *Development* section of the project website.

[https://www.haiku-os.org/development/getting-started](https://www.haiku-os.org/development/getting-started)

[https://www.haiku-os.org/development](https://www.haiku-os.org/development)

[https://www.haiku-os.org/development/coding-guidelines](https://www.haiku-os.org/development/coding-guidelines)

### How do I create and submit patches?

After having checked out our repository and configured git you can modify the source files. Always check if your modifications compile without errors/warnings. To create and submit a patch, please see the [development wiki on patches](https://dev.haiku-os.org/wiki/CodingGuidelines/SubmittingPatches) (external link).

[https://www.haiku-os.org/guides/building](https://www.haiku-os.org/guides/building)

[https://www.haiku-os.org/guides/building/get-source-git](https://www.haiku-os.org/guides/building/get-source-git)

[https://dev.haiku-os.org/wiki/CodingGuidelines/SubmittingPatches](https://dev.haiku-os.org/wiki/CodingGuidelines/SubmittingPatches)

### What development tools do you use?

A heavily modified version of [Jam](http://www.perforce.com/jam/jam.html) as our building tool. It is included in Haiku's official releases and nightly images. If you are cross-compiling Haiku, you will need to build jam from source.

[Git](http://git-scm.com/) as our version control system.

[Trac](https://dev.haiku-os.org/) as our project management and bug/issue tracking system.

[Gerrit](https://review.haiku-os.org/) for code review.

[https://www.haiku-os.org/development/faq#dev-tools](https://www.haiku-os.org/development/faq#dev-tools)

Mailing list

[https://www.haiku-os.org/community/ml](https://www.haiku-os.org/community/ml)

IRC

[https://www.haiku-os.org/community/irc](https://www.haiku-os.org/community/irc)