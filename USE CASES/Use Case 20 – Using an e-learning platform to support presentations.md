Use Case 20 – Using an e-learning platform to support presentations.md
=========================================================
When presenting software at conferences or seminars it is easy to demonstrate the functionalities, but much more difficult to effectively communicate the actual user experience. Furthermore, the passive mode of listing makes it easier to forget what the software could do or how to do it. In order to engage the participants, online services can be provided where the software is installed and examples are available, allowing the participants to get hands on experience and work with problems of their own choice. Such practical experience makes it more likely the participants would remember the software and provide a starting point for using it.

This approach was tested at a recent seminar held at MLZ where the WP5 software McStasScript and the McStas Union components were presented. After the seminar the participants could follow a link to the PaNOSC WP8 e-learning portal pan-learning.org where tutorials were deployed in Jupyter notebooks, eliminating the need for any setup on the participants computers. The feedback was highly positive as it gave a more clear picture of both what the software could do and how this was accomplished in practice.

Main Contributors
------
* **Mads Bertelsen**, ([ESS, European Spallation Source](https://europeanspallationsource.se/) – Wrote McStasScript / Union components and presented at MLZ virtual seminar.
* **Peter Link**, ([MLZ](https://mlz-garching.de/)) – Requested seminar on advanced McStas use.
* **Peter Willendrup**, [ESS](https://europeanspallationsource.se/) / [Technical University of Denmark, DTU](https://www.dtu.dk/english)) Main McStas developer and administration of e-learning platform

Use Case Action Flow
------
* Setup e-learning content for subject: Add course material to an e-learning platform describing the software to be presented.
* Prepare demo accounts for participants: Setup demo accounts that can be distributed to participants or allow anonymous access to the e-learning content.
* Present the software: Present the software through seminar, conference talk or similar, ending with brief instructions on how to access the e-learning material.
* Interactive session for participants: The participants can now access the e-learning material, in a seminar setting it may be possible to ask the developer questions directly.

Description of needs
------
The main requirement is the e-learning platform, which needs to support Jupyter notebooks and have sufficient computational resources available. In addition interesting course material, tutorials or similar need to be contributed to the platform by the speaker. The ability to create temporary demo accounts or provide the platform in an open area is also necessary.

Impacts from the implementation
------
Efficient decimation of new software, making it an interactive experience for participants. More likely to attract new users of the software.

Generalisation of use case
------
Due to the broad appeal of e-learning, the concept can be used in a broader sense. For example if an instrument concept is presented, an e-learning course that includes simulation of the instrument could be provided. This would allow participants to perform sample experiments and see the data quality for cases relevant to them.

Resources
------
Used e-learning platform:
* https://pan-learning.org
* https://github.com/pan-training
* Presented software, including Jupyter notebook tutorials. https://github.com/PaNOSC-ViNYL/McStasScript

Contact person
------
[**Mads Bertelsen**](mailto:mads.bertelsen@ess.eu) (European Spallation Source)
