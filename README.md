Ghost CEH 
=================
An Edited Release Version of Ghost by caleuanhopkins

## WARNING

Extra custom core file edits for Ghost Blog which add extra features to the public release version of Ghost blogging platform. This repo has no affiliation to the official Ghost repo, and it in no way supported or recognised by the Ghost development team. USE AT YOUR OWN RISK.

## About

Ghost is an amazing blogging platform that's taking the blogging sphere by storm. Ghost is an open source platform, and allows developers to build upon its core to create their own versions of Ghost to use privately.

This repo contains a personally edited edition of Ghost which I (caleuanhopkins) have done to match the wants and needs I wish to have in the Ghost blogging platform. This version is not supported or has any affiliation to the official Ghost Foundation version of Ghost, nor to its development team. This is strictly for personal and experimentation purposes only.

## Features

### Post Images & Global Vars - 25/11/2013

Been working on a quick and dirty solution to get post images working as my CEH theme needed them. Not only that, but for the social media head meta tags, I needed some global variables to work outside the post loop. Thankfully, I got both to work, but it's worth noting that the Post Images only work by **URL only**. So no image uploader feature installed, it will only work by typing or pasting in the image url. Here's a quick GIF:

!(http://i.imgur.com/B2MUFzp.gif?1)

### Installation

### Git Clone

The eaisest way to get started with this version is to clone the repo to your server or local enviroment:

    git clone https://github.com/caleuanhopkins/ghost-ceh-release.git
    
This repo has no `content` directory or sub directories so customer themes and data is not overwritten if this repo is cloned to and exsisting Ghost instance. If you don't already have Ghost or this diretcory on your local enviroment or on the server you plan to clone this repo to, please grab a copy of it from either the [Ghost repo](https://github.com/TryGhost/Ghost) or a copy from the [Ghost release](https://ghost.org/download/) version.

### Manual Upggrade / Installation

If you want to update the files by hand, you can do so by downloading this repo or and copying the following files from this repo to your Ghost enviroment:

* core/server/views/editor.hbs
* core/client/assets/css/screen.css
* core/server/helpers/index.js
* core/client/views/editor.js
* core/built/scripts/views.js
* core/built/scripts/ghost.js

These files in this repo contain the updated core to allow Post Images to work in the Ghost admin panel and for the post images and allows you to use the following global vars anywhere in your theme:

`{{theURL}}` - Give the URL for a post. useful for meta tags.
`{{postImage}}` - The URL of the post image.

=================

## Copyright & License

**GHOST CEH**

Copyright (C) 2013 - Released under the MIT License.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.