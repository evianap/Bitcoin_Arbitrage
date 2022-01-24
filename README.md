# bitcoin_arbitrage
[![LinkedIn][linkedin-shield]][linkedin-url]
<!-- [![License][license-shield]][license-url] -->

<!-- PROJECT LOGO -->
<br />
<p align="center">
    <img src="" alt="Bitcoin" width="700" height="300">
  </a>

  <h3 align="center">bitcoin_arbitrage_</h3>

  <p align="center">
    Finding Arbitrage Opportunities for Bitcoin
    <br />
    <a href="https://github.com/evianap/bitcoin_arbitrage"><strong>Go to documents »</strong></a>
    <br />
  </p>
</p>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
      </ul>
    </li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

<p>This project is designed to download data series from a csv file with historic market prices of bitcoin from different marketplaces. With these files, the program will analyze data for specific dates to find arbitrage opportunities:<p/>

```
bitstamp_df = bitstamp_dataframe=pd.read_csv(
    Path('./Resources/bitstamp.csv'),
    index_col="Timestamp",
    parse_dates=True,
    infer_datetime_format=True
)
```
<p align="center"><img src="" alt="series_screenshot" width="450" height="650"><p/>

<p>In the sample dates that were randomly selected, no profitability was found<p/>

```
# Create an overlay plot that visualizes the two dataframes over a period of one day early in the dataset. 
# Be sure that the plots include the parameters `legend`, `figsize`, `title`, `color` and `label` 
# YOUR CODE HERE

bitstamp_sliced['Close'].loc['2018-01-02'].plot(legend=True, figsize=(10,6), title="Bistamp vs Coinbase Jan 2nd 2018", color="blue", label="Bitstamp")
coinbase_sliced['Close'].loc['2018-01-02'].plot(legend=True, figsize=(10,6), color="Orange", label="Coinbase")
```


<p align="center"><img src="" alt="screenshot_error_" width="550" height="200"><p/>


### Built With

<!-- This section should list any major frameworks that you built your project using. Leave any add-ons/plugins for the acknowledgements section. Here are a few examples. -->

* [Python](https://www.python.org/)
* [Jupyter Lab](https://jupyter.org/install)

### Prerequisites

<!-- This is an example of how to list things you need to use the software and how to install them. -->
A variety of libraries were used and are needed for this program. They can be added using the below commands in terminal:

``` 
import pandas as pd
from pathlib import Path
%matplotlib inline
import numpy as np
```



<!-- CONTACT -->
## Contact

Enrique Viana - [@evianap][linkedin-url] - j.enrique.viana@gmail.com

Project Link: [https://github.com/evianap/bitcoin_arbitrage](https://github.com/evianap/bitcoin_arbitrage)

<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements

* [Kevin Lee](https://github.com/kevinclee26/)
* [Hitarth Smart](https://github.com/smarthitarth)
* [Sajal Sharma](https://github.com/sajal-sharma)

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

<!-- [license-shield]: 
[license-url]:  -->
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/enriqueviana/