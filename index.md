---
title: Licensing your code
...

# Licensing your code

<style> .reveal h1 { font-size: 2em; } </style>

Why, when and how.

(This is software engineering advice, and has not been checked by a legal expert.)

# Hi, I'm [Bob](https://rse.shef.ac.uk/contact/bob-turner/)!

Career...
Software Consultant -> Researcher -> Research Software Engineer

<!--This can be modified for individual presenters-->

# RSE at Sheffield

![RSE](https://github.com/RSE-Sheffield/RSE-Sheffield.github.io/raw/master/assets/images/logo/rse-logoonly-stroke.png){ height=256px }

13 RSEs, 35 projects / year worth ~£11m total

# Operational Model

- Underwritten by overheads
- Funded from external sources

# Results

- Financial sustainability
- “Fair” allocation of staff to projects
- “Convenient” access to growing pool of expertise and experience
- (Mainly) academic led
- Open ended contracts for RSEs

# Talk Structure

- Definitions
- Examples of open source software
- Ideological motivation
  - FAIR
  - Four Freedoms
- Barriers to open sourcing
- How to open source

# Copyright

[Berne Convention](https://en.wikipedia.org/wiki/Berne_Convention) of 1886: Copyright is immediately bestowed upon a work the moment it is created, without requiring any registration.

# License

Relaxes conditions imposed by copyright in specific ways.

# Examples of open source

::: incremental

* Linux
* Firefox
* Python
* VSCode (Microsoft)
* PyTorch (Facebook)

:::

# Motivation: FAIR Priniciples

![](https://the-turing-way.netlify.app/_images/fair-principles.jpg){ height=300px }

The Turing Way project illustration by Scriberia. Used under a CC-BY 4.0 licence. DOI: 10.5281/zenodo.3332807.

# Is software a special type of data?

::: incremental

- Yes
- But...
  - Executable
  - Changes a lot

:::

# FAIR4RS: We envision a world where:

* All research is reproducible
* All research software is open
* All research software is usable by others (for their own research)
* All contributors to research software are recognized for their work
* All research software is sustained as long as it is useful
* All research software is high-quality and robust

[Katz et al. 2021](https://arxiv.org/ftp/arxiv/papers/2101/2101.10883.pdf)

# [Four freedoms (abridged)](https://www.gnu.org/philosophy/free-sw.en.html)

- The freedom to run the program as you wish, for any purpose (freedom 0).
- The freedom to study how the program works, and change it so it does your computing as you wish (freedom 1).
- The freedom to redistribute copies so you can help others (freedom 2).
- The freedom to distribute copies of your modified versions to others (freedom 3).

# National Policy

![](images/roadmap.png)

[https://www.gov.uk/government/publications/uk-research-and-development-roadmap](https://www.gov.uk/government/publications/uk-research-and-development-roadmap)

# Reasons **not** to make code open

::: incremental

- Wait for publication
- Want to commercialise
- Don't have permission (e.g. co-authors / collaborations)
- Shyness / fear

:::

# Wait for publication...

Fear of scoop by a competing group.

::: incremental

- Open code:
  - Faster impact
  - More eyes, less bugs

:::

# Want to commercialise...

Open source software is compatible with capitalism.

Explore options for spin outs / licensing early (*Research Services Impact & IP Team*).

# Don't have permission...

::: incremental

- Ask for permission from co-authors.
- Check what project-specific restrictions are in place.

:::

# Shyness / fear

::: incremental

- "My code isn't good enough."
- "My code isn't valuable."

:::

# How to open source

::: incremental

- Choose a licence, agreed by everyone on the project.
- Put the licence text in a file alongside your code.
- Publish your code somewhere such as GitHub or GitLab.
- *Release a package.*
- *Reference specific versions using [ORDA](https://orda.shef.ac.uk/), [Zenodo](https://zenodo.org/) or equivalent.*

:::

# Choose a license

:::::::::::::: {.columns}
::: {.column width="50%"}
**"Copyleft"** e.g. [GPL3](https://choosealicense.com/licenses/gpl-3.0/) - better for academic collaboration
:::
::: {.column width="50%"}
**More permissive** e.g. [MIT](https://choosealicense.com/licenses/mit/) - better for private sector collaboration
:::
::::::::::::::

[choosealicence.com](https://choosealicense.com/)

*Presenter follow links.*

# Apply the licence

![](images/license-file.png)

- Most licenses require a single file like `LICENSE` or `LICENSE.txt`.
- Some licences advise that you should put a message at the top of every file.

# Publish

![](images/auto-license.png){ height=512px }

# Even FAIRer?

![](images/fairpusher.svg){ height=512px }

<!--
graph TD
    A[GitHub] -->|Webhook or action| B(Package Index - PyPI, CRAN, ...)
    A -->|Webhook or action| C(Archive - ORDA, Zenodo, ...)
-->

# Draft guidance

![](https://mermaid.ink/img/eyJjb2RlIjoiZmxvd2NoYXJ0IFREXG4gICAgQShbV2lsbCB5b3UgaW5jbHVkZSBjb2RlIGZyb20gcGVvcGxlIG91dHNpZGUgdGhlIHByb2plY3Q_XSlcbiAgICBCKFtEb2VzIG5vbi1wcm9qZWN0IGNvZGUgYWxsb3cgcmUtbGljZW5zaW5nP10pXG4gICAgQyhbRG9lcyBmdW5kZXIgcmVxdWlyZSBhIHNwZWNpZmljIGxpY2Vuc2U_XSkgICAgXG4gICAgRChbV2FzIG9wZW4gc291cmNlIGxpY2Vuc2luZyBzcGVjaWZpZWQgaW4gdGhlIGZ1bmRpbmcgYXBwbGljYXRpb24_XSkgICAgXG5cbiAgICBFKFtJcyB0aGVyZSBhIGNvbW1lcmNpYWwgb3Bwb3J0dW5pdHk_XSlcbiAgICBGKGh0dHBzOi8vd3d3LnNoZWZmaWVsZC5hYy51ay9ycy9jb21tZXJjaWFsaXNhdGlvbi9pY2UtZm9ybSlcblxuICAgIEcoVXNlIGFuIGFwcHJvcHJpYXRlIG9wZW4gc291cmNlIGxpY2Vuc2UuKVxuICAgIEgoU2VlayBhc3Npc3RhbmNlIGZyb20gbGlicmFyeSAvIFJTRS4pXG4gICAgSShVc2UgbGljZW5zZSBzdGlwdWxhdGVkIGJ5IGZ1bmRlci4pXG5cbiAgICBKKFtEb2VzIHRoZSBjb21tZXJjaWFsIG9wcG9ydHVuaXR5IHByZWNsdWRlIG9wZW4gc291cmNlIGxpY2VzbmluZz9dKVxuXG4gICAgSyhDbG9zZWQgc291cmNlLilcblxuICAgIEEgLS0-fFllc3wgQlxuICAgIEIgLS0-fE5vfCBIXG4gICAgQiAtLT58WWVzfCBDXG4gICAgQSAtLT58Tm98IENcbiAgICBDIC0tPnxZZXN8IElcbiAgICBDIC0tPnxOb3wgRFxuICAgIEQgLS0-fFllc3wgR1xuICAgIEQgLS0-fE5vfCBFXG4gICAgRSAtLT58WWVzfCBGXG4gICAgRiAtLT4gSlxuICAgIEogLS0-fE5vfCBHXG4gICAgRSAtLT58Tm98IEdcbiAgICBKIC0tPnxZZXN8IEsiLCJtZXJtYWlkIjp7InRoZW1lIjoiZGFyayJ9LCJ1cGRhdGVFZGl0b3IiOmZhbHNlLCJhdXRvU3luYyI6dHJ1ZSwidXBkYXRlRGlhZ3JhbSI6ZmFsc2V9){ height=512px }

# Thank you

# University of Sheffield advice

- [Research Software Engineering team **Code Clinic**](https://rse.shef.ac.uk/)
- [Library, Research Data Management](https://www.sheffield.ac.uk/library/rdm)
- [Research Services Impact & IP Team](https://www.sheffield.ac.uk/rs/impact)