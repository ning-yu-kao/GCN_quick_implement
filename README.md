<div id="top"></div>



<!-- PROJECT SHIELDS -->

[![MIT License][license-shield]][license-url]
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ning-yu-kao)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kaoningyupage/)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kaoningyu@gmail.com)
[![Medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)]()





<!-- PROJECT LOGO -->
<br />
<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1y2FQhbDwmuvp2WvxkuuEDYmYiwEo69iD" width="500" height="300">
  <h1 align="center">Predict Protein-protein Interaction Network using Graph Convolutional Network (GCN)</h1>
  <p>Understanding functions of proteins in specific human tissues is essential for insights into
disease diagnostics and therapeutics, yet prediction of tissue-specific cellular function remains a critical
challenge for biomedicine. However, the interactions between proteins was not only a sigle connection. The protein-protein interaction (PPI) between proteins are influcing each other as a network called PPI network. Thus, advance technology was needed to discover the information in these complex structures. This project is a quick inplementaion of Graph Convolutional Network using the PPI dataset.</p>
</div>



<!-- TABLE OF CONTENTS -->
<details open>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#license">License</a></li>
    <li><a href="#references">References</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

Although incredibly influential, current methods for protein function prediction lack tissue specificity as they assume that protein functions are constant across organs and tissues. Our goal is to learn features of proteins in different tissues. We represent each tissue as a network, where nodes represent proteins. 


### Built With

This is major frameworks/libraries used in this project.

* Python
* [Pytorch](https://pytorch.org/)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

Please follow the instruction below to set up your environment.

### Installation


1. Install packages

  * **PyG (PyTorch Geometric)**
   
    <img height="100" src="https://raw.githubusercontent.com/pyg-team/pyg_sphinx_theme/master/pyg_sphinx_theme/static/img/pyg_logo_text.svg?sanitize=true">
    
    > A library built upon PyTorch to easily write and train Graph Neural Networks (GNNs) for a wide range of applications related to structured data.
    
    You can just use `pip` or `conda` to install PyG. However, I would higly recommend installing with `conda`.(So many errors occur when I using `pip`)
    
    1. Visit to install PyTorch first
    
    ```bash
    pip install pystan==2.19.1.1
    pip install prophet
    ```
     
    For more installation detail, please check out [PROPHET](https://facebook.github.io/prophet/docs/installation.html#installation-in-python) official website.

<p align="right">(<a href="#top">back to top</a>)</p>

  * **Yahoo! Finance's API**
    
    > It's an open-source tool that uses Yahoo's publicly available APIs, and is intended for research and educational purposes.
    
    ```bash
    pip install yfinance
    ```
    
    Quick start to fatch stock data:
    
    ```python
    import yfinance as yf
    data = yf.download("SPY AAPL", start="2017-01-01", end="2017-04-30")
    ```



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>


## References
```bash
@article{prophet,
author = {Taylor SJ, Letham B.}
title = {Forecasting at scale},
journal = {PeerJ Preprints},
year = {2017},
doi = {https://doi.org/10.7287/peerj.preprints.3190v2},
}
```

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

These resources are which I would like to give credit to.
* [Time Series Forecasting With Prophet in Python](https://machinelearningmastery.com/time-series-forecasting-with-prophet-in-python/)
* [Free Stock Data for Python Using Yahoo Finance API](https://towardsdatascience.com/free-stock-data-for-python-using-yahoo-finance-api-9dafd96cad2e)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTACT -->
## Contact
<div align="center">
  <h3>Please feel free to connect with me on social media</h3>
    <a href="https://github.com/ning-yu-kao">
        <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-social-github.png" width="3%"/>
    </a>
    <img width="3%" />
    <a href="https://www.linkedin.com/in/kaoningyupage">
        <img src="https://github.com/ultralytics/yolov5/releases/download/v1.0/logo-social-linkedin.png" width="3%"/>
    </a>
    <img width="3%" />

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/ning-yu-kao/GCN_quick_implement/blob/main/LICENSE
