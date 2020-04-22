# lmm333's slice

Host lmm333's slice online, most slices run by reveal.js and image host on qiniu.com

## Usage

1. Copy base html files from /templete to new folder
2. Update <title> , add .md files
3. Publish to github
4. [Optional] If want to preview md files locally, need to setup npm server, see **Preview md on localhost** below or see README.md file under `reveal.js-3.6.0` for more detail

## reveal.js

A framework for easily creating beautiful presentations using HTML. [Check out the live demo](http://revealjs.com/).

## Preview Markdown on localhost
1. Make sure finish Full setup first
1. Copy .md and image files to `reveal.js-3.6.0` folder and update md file name in external_md.html
1. Serve the presentation and monitor source files for changes
   ```sh
   $ cd reveal.js-3.6.0
   $ npm start
   ```
1. Open `http://localhost:8000/external_md.html`

## Full setup

Some reveal.js features, like external Markdown and speaker notes, require that presentations run from a local web server. The following instructions will set up such a server as well as all of the development tasks needed to make edits to the reveal.js source code.

1. Install [Node.js](http://nodejs.org/) (4.0.0 or later)

1. Clone the reveal.js repository
   ```sh
   $ git clone https://github.com/hakimel/reveal.js.git
   ```

1. Navigate to the reveal.js folder
   ```sh
   $ cd reveal.js
   ```

1. Install dependencies
   ```sh
   $ npm install
   ```

1. Serve the presentation and monitor source files for changes
   ```sh
   $ npm start
   ```

1. Open <http://localhost:8000> to view your presentation

   You can change the port by using `npm start -- --port=8001`.

## qiniu.com

A cloud computering website, I am using image CDN storage of it, [imageView2 API document](https://developer.qiniu.com/dora/manual/1279/basic-processing-images-imageview2)

Add image to md like below, use <!-- .element --> to control image size


    ![](http://7xinjz.com1.z0.glb.clouddn.com/travel/180719slices/Cambodia00.JPG?imageView2/2/w/2000) <!-- .element height="90%" width="90%" -->


## License

MIT licensed

Copyright (C) 2018 lmm333, http://lmm333.com/

## 注意
- 相对路径插入图片，使用 ![](images/a.JPG)
   - 注意images前面没有/ 否则会变成 lmm333.com/images/a.JPG 的绝对路径
   - 注意照片后缀名的大小写敏感，建议全部重命名为小写，避免麻烦