# lmm333's slice

Host lmm333's slice online, most slices run by reveal.js and image host on qiniu.com

## Usage

1. Copy base html files from /templete to new folder
2. Update <title> , add .md files
3. Publish to github
4. [Optional] If want to preview md files locally, need to setup npm server, see README.md file under /reveal.js-3.6.0 for more detail

## reveal.js

A framework for easily creating beautiful presentations using HTML. [Check out the live demo](http://revealjs.com/).

## qiniu.com

A cloud computering website, I am using image CDN storage of it, [imageView2 API document](https://developer.qiniu.com/dora/manual/1279/basic-processing-images-imageview2)

Add image to md like below, use <!-- .element --> to control image size


    ![](http://7xinjz.com1.z0.glb.clouddn.com/travel/180719slices/Cambodia00.JPG?imageView2/2/w/2000) <!-- .element height="90%" width="90%" -->


## License

MIT licensed

Copyright (C) 2018 lmm333, http://lmm333.com/
