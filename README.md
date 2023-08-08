OFX Parser is a PHP library designed to parse an OFX file downloaded from a financial institution into simple PHP objects. 

It supports multiple Bank Accounts, the required "Sign On" response, and recognises OFX timestamps.

## Installation

Simply require the package using [Composer](https://getcomposer.org/):

```bash
$ composer require mehmetcoban/ofxparser
```

## Usage

You can access the nodes in your OFX file as follows:


Most common nodes are support. If you come across an inaccessible node in your OFX file, please submit a pull request!


Investments look much different than bank / credit card transactions. This version supports a subset of the nodes in the OFX 2.0.3 spec, per the immediate needs of the author(s). You may want to reference the OFX documentation if you choose to implement this library. In particular, this does not currently process investment positions (INVPOSLIST) or referenced security definitions (SECINFO).


To load investments from a Quicken (QFX) file or a MS Money (OFX / XML) file:
