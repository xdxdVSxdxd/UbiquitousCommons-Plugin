# Ubiquitous Commons - Chrome Plugin

Welcome to the first implementation of the Ubiquitous Commons.

It comes under the form of a Chrome Plugin (Firefox and other browsers coming soon).

It is designed to intercept all generation you generate on social networks and other online services (such as GMail, Twitter etc.), encrypt it, send it to the service provider (Facebook, Google, Twitter, etc) in encrypted form, and declare the allowed usages through a polymorphic license, through which you are able to choose the ways in which you allow usage of the information you generated (for a series of people, for a purpose, for science, etc.).

The Licence and is then placed on the Blockchain, so that your information becomes usable only through the pugin itself, and only if you are included in the allowances of the license.

That's it! You instantly have the tool to make sure that your information is used only the way you intend to, and also to promote your desired usage for your information (for a certain cause? for civic action? for governance? for science? you decide).


# Ubiquitous Commons

To know more about Ubiquitous Commons project: http://www.ubiquitouscommons.org/

The Ubiquitous Commons is an international research effort dedicated to understanding the transformation of data, information and knowledge in the age of ubiquitous technologies.

It is dedicated to creating tools and practices through which citizens, institutions, organizations, enterprises, researchers and other stakeholders can enact shared, participatory and ethical processes in which all subjects become actively engaged in defining how the data and information they produce (through their bodies, expressions, movements, actions, gestures…) are used, making sure that their rights are protected and that ethical initiatives for science, civic action, social organization and coordination become possible and desirable.


# the Plugin

The development of the plugin is still in Alpha. Most things already work, but don't expect a finished product (yet).

This project uses Ethereum as a Blockchain application layer.

To get it running:


0) install Ethereum

https://dev.ethereum.org/



1) Run an ethereum local node

look at:
https://github.com/ethereum/cpp-ethereum/wiki/Local-Test-Net

(we need an Ethereum local node for now, because we don't yet have a blockchain running, until we finish a decent testing phase)



2) Install ethereum.js


- if you have node installed:
npm install ethereum.js

- otherwise just go at:

https://github.com/ethereum/ethereum.js/


3) configure

- grab the latest ethereum.js (at step 2) and paste it to the ext folder in this repository

- search for "web3.setProvider(new web3.providers.HttpProvider('http://localhost:8545'));" in "background.js" and replace the URL with the URL for your local ethereum node


4) Install the Chrome extension:

- enable "Developer tools" in your Chrome browser.

- go to the "Extensions" menu in the options screen

- choose "Load unpacked extension"

- browse to the "uc-plugin/ext" in this repository and click "open"

your plugin is installed



As of now you are only running on a local blockchain, but the steps are all there.

There's a trick, to understand if everything is working, in which you can grab the licenses and keys contained in the options screen of the plugin, and past them to another instance, so that you can see if everything works.

Obviously this feature will be completely removed in the near (near) future.

It also works if you run in a local network in which a ethereum node is running.