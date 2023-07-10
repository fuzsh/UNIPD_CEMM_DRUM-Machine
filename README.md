<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/farzad-845/UNIPD_CEMM_DRUM-Machine">
    <img src="images/pure-data.png" alt="Logo" width="140" height="80">
  </a>

<h3 align="center">Drum Machine Step Sequencer (Pure Data)</h3>

  <p align="center">
    A drum machine step sequencer is a device or software application used in music production to create and program rhythmic patterns for electronic drum sounds. It is a fundamental tool in electronic music production and is often found in hardware drum machines or as a feature in software-based music production environments.
    <br />
    <a href="https://github.com/farzad-845/UNIPD_CEMM_DRUM-Machine"><strong>Explore the docs »</strong></a>
    <br />
    <br />    ·
    <a href="https://github.com/farzad-845/UNIPD_CEMM_DRUM-Machine/issues">Report Bug</a>
    ·
    <a href="https://github.com/farzad-845/UNIPD_CEMM_DRUM-Machine/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li><a href="#license">License</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project
![Drum Machine Step Sequencer (Pure Data)][product-screenshot]
- General Workflow:
  - Active DSP
  - we have bangs for each sound that receive a signal from the sequencer and then read the wav file;
  - send the read file to dac~ to convert the digital file to analog.
- Inside Main Sequencer:
  - There is a toggle that receives a signal for playing or stopping the process;
  - This toggle activates each individual sequence in a connected way.
- Inside Each Sequencer (for each sound):
  - There is an 8-step sequencer;
  - The counter sends a signal to 8 different 'bangs' that then go back to the primary sequencer process;
  - we use spigot to allow the signal through only if the related toggle is on.
<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With

* [![PureData][PureData.pd]][PureData-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

#### Contributors
- Mirco Cazzaro
- Nicola Boscolo Cegion
- Farzad Shami

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/farzad-845/UNIPD_CEMM_DRUM-Machine.svg?style=for-the-badge
[contributors-url]: https://github.com/farzad-845/UNIPD_CEMM_DRUM-Machine/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/farzad-845/UNIPD_CEMM_DRUM-Machine.svg?style=for-the-badge
[forks-url]: https://github.com/farzad-845/UNIPD_CEMM_DRUM-Machine/network/members
[stars-shield]: https://img.shields.io/github/stars/farzad-845/UNIPD_CEMM_DRUM-Machine.svg?style=for-the-badge
[stars-url]: https://github.com/farzad-845/UNIPD_CEMM_DRUM-Machine/stargazers
[issues-shield]: https://img.shields.io/github/issues/farzad-845/UNIPD_CEMM_DRUM-Machine.svg?style=for-the-badge
[issues-url]: https://github.com/farzad-845/UNIPD_CEMM_DRUM-Machine/issues
[license-shield]: https://img.shields.io/github/license/farzad-845/UNIPD_CEMM_DRUM-Machine.svg?style=for-the-badge
[license-url]: https://github.com/farzad-845/UNIPD_CEMM_DRUM-Machine/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/farzad-shami
[product-screenshot]: images/screenshot.png
[PureData.pd]: https://img.shields.io/badge/puredata-000000?style=for-the-badge&logo=puredata&logoColor=white
[PureData-url]: https://puredata.info/



---

<p><em>Computer Engineering for Music and Multimedia course of <a href="http://www.unipd.it">University of Padova</a></em>
