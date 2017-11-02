# docker-phantomjs-ja

## Features of this image

Build from [docker-phantomjs](https://github.com/wernight/docker-phantomjs) with Japanese Font.

## Usage

### JavaScript interactive shell
 
Start PhantomJS in [REPL](http://phantomjs.org/repl.html):

    $ docker run --rm wernight/phantomjs
    >

### Remote WebDriver

Start as 'Remote WebDriver mode' (embedded [GhostDriver](https://github.com/detro/ghostdriver)):

    $ docker run -d -p 8910:8910 wernight/phantomjs phantomjs --webdriver=8910

### Screenshot

Take a Screenshot:

    $ docker run -v $(pwd):/data tkikuchi/phantomjs-ja /srv/var/phantomjs/examples/rasterize.js http://example.com /data/example.com.png
