This repository was originally cloned from https://github.com/rounakbanik/generative-art-nft.

# Generative NFT Script

## Introduction

The `generative-art-script` repository is a library for creating generative art. It was developed for the purpose of creating NFT avatar & collectible projects.

## Features

### Generate over a million distinct images with less than 60 traits
The library allows you to generate images every distinct possible combination of your traits. For context, if you had trait art for a project like [Bored Apes](https://boredapeyachtclub.com/#/home), the library could generate upwards of 1.2 billion distinct apes.

### Add rarity weights
The library also allows you to configure the image generation process in such a way that you have complete control over how rare each and every trait is.

### Generate compliant JSON metadata for your NFTs
There is now an added functionality to generate JSON metadata for your NFTs that are in compliance with OpenSea metadata requirements (and by extension, the general NFT metadata standard).

## Installation

**Clone this repository**

```shell
git clone https://github.com/nova-network-inc/generative-nft-script.git
```

**Install required packages**

```shell
pip install Pillow pandas progressbar2
```

Upload your input assets in the `assets` folder, fill up the `config.py` file, and then run:

```shell
python nft.py
```

In order to generate JSON metadata, define `BASE_NAME, BASE_IMAGE_URL`, and `BASE_JSON` in `metadata.py` and then run:

```shell
python metadata.py
```
