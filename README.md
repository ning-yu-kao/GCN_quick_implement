<div id="top"></div>



<!-- PROJECT SHIELDS -->

[![MIT License][license-shield]][license-url]
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ning-yu-kao)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kaoningyupage/)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kaoningyu@gmail.com)
[![Medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@kaoningyu/introduction-of-graph-convolutional-network-gcn-quick-implementation-5dd75e75b261)





<!-- PROJECT LOGO -->
<br />
<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1y2FQhbDwmuvp2WvxkuuEDYmYiwEo69iD" width="500" height="300">
  <h1 align="center">Predict Protein-protein Interaction Network using Graph Convolutional Network (GCN)</h1>
  <p>Understanding functions of proteins in specific human tissues is essential for insights into
disease diagnostics and therapeutics, yet prediction of tissue-specific cellular function remains a critical
challenge for biomedicine. However, the interactions between proteins was not only a sigle connection. The protein-protein interaction (PPI) between proteins are influcing each other as a network called PPI network. Thus, advance technology was needed to discover the information in these complex structures. This project is a quick inplementaion of Graph Convolutional Network using the PPI dataset.</p>
</div>

***If you need information about GCN, please check out my Medium article about introduction to GCN through the Medium badge on the top***

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
    
    1. Visit [PyTorch website](https://pytorch.org/get-started/locally/) to install PyTorch first
    
        Select your OS/PyTorch/CUDA combination and install, for me it's:


        ```bash
        conda install pytorch torchvision torchaudio cudatoolkit=11.3 -c pytorch
        ```
      
    2. Install PyG
        ```bash
        conda install pyg -c pyg
        ```
        
    3. Check installation
        To check if you install PyG successfully, run this code:
        
        ```python
        import torch
        import torch_geometric.transforms as T
        from torch_geometric.datasets import PPI
        from torch_geometric.loader import DataLoader
        from torch_geometric.nn import GCN2Conv
        ```
    For more installation detail, please check out [PyG](https://github.com/pyg-team/pytorch_geometric) official GitHub repository.

    

  * **Weights & Biases**
  
    <img src="https://drive.google.com/uc?export=view&id=1VdTXrUtR2ero3XCN1v4QLuCcw23KZFa5" width="300" height="50">
    
    > Weights & Biases is the MLOps platform for developers to build and monitor their model status.

    1. You can simply install it by:
    
        ```bash
        pip install wandb
        ```
    
    2. Sign up an account in [W&B website](https://wandb.ai/site). 
    
    3. Test this code with your [API key](https://wandb.ai/authorize).
    
        ```python
        wandb.login(anonymous="must", key='Your Key')
        print("Successfully Logged In!")
        ```
        
     You guys can view my output dashboard of a sigle run at this [link](https://wandb.ai/kaoningyu/gcn-ppi/reports/Predict-PPI-network-using-GCN--VmlldzoyMDIyNDgw?accessToken=0fgywscyq72iiivoyiq1lunofjhvkdqbejovoug456owxpjkax4ize40ug7wtwtr).
     
<p align="right">(<a href="#top">back to top</a>)</p>


<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>


## References
```txt
@article{Zitnik2017,
  title={Predicting multicellular function through multi-layer tissue networks},
  author={Zitnik, Marinka and Leskovec, Jure},
  journal={Bioinformatics},
  volume={33},
  number={14},
  pages={190-198},
  year={2017}
}

@inproceedings{Fey/Lenssen/2019,
  title={Fast Graph Representation Learning with {PyTorch Geometric}},
  author={Fey, Matthias and Lenssen, Jan E.},
  booktitle={ICLR Workshop on Representation Learning on Graphs and Manifolds},
  year={2019},
}

@article{kipf2016semi,
  title={Semi-supervised classification with graph convolutional networks},
  author={Kipf, Thomas N and Welling, Max},
  journal={arXiv preprint arXiv:1609.02907},
  year={2016}
}
```


<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

These resources are which I would like to give credit to.
* [Graph Convolutional Networks](https://tkipf.github.io/graph-convolutional-networks/)
* [Feature Learning in Multi-Layer Networks](http://snap.stanford.edu/ohmnet/)

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
