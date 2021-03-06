
---
title: 纯CSS3实现多列的瀑布流布局 
date: 2017-10-17 14:51:01
tags:
- CSS3 
- CSS
categories: 
- CSS 
---


## 纯CSS3实现多列的瀑布流布局 
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>纯CSS3实现多列的瀑布流布局 </title>
</head>
<style type="text/css" media="screen">
body {
    background-color: #f6f6f6;
}

.container {
    width: 80%;
    margin: 0 auto;
}

.waterfall {
    -moz-column-count: 3;
    -webkit-column-count: 3;
    column-count: 3;
    -moz-column-width: 24em;
    -webkit-column-width: 24em;
    column-width: 24em;
    -moz-column-gap: 1em;
    -webkit-column-gap: 1em;
    column-gap: 1em;
}

.pin {
    padding: 1em;
    margin: 0 0.125em 1em;
    -moz-page-break-inside: avoid;
    -webkit-column-break-inside: avoid;
    break-inside: avoid;
    background: white;
    -moz-box-shadow: 0 1px 3px 0 rgba(0, 0, 0, 0.12), 0 1px 2px 0 rgba(0, 0, 0, 0.24);
    -webkit-box-shadow: 0 1px 3px 0 rgba(0, 0, 0, 0.12), 0 1px 2px 0 rgba(0, 0, 0, 0.24);
    box-shadow: 0 1px 3px 0 rgba(0, 0, 0, 0.12), 0 1px 2px 0 rgba(0, 0, 0, 0.24);
}

.pin img {
    width: 100%;
    padding-bottom: 1em;
    margin-bottom: 0.5em;
    border-bottom: 1px solid #cccccc;
}
</style>

<body>
    <div class="container">
        <div class="waterfall">
            <div class="pin">
                <img src="http://dummyimage.com/640x4:3" />
                <p>1 convallis timestamp</p>
            </div>
            <div class="pin">
                2 Donec a fermentum nisi.
            </div>
            <div class="pin">
                <img src="http://dummyimage.com/640x3:4" />
                <p>
                    3 Nullam eget lectus augue. Donec eu sem sit amet ligula faucibus suscipit. Suspendisse rutrum turpis quis nunc convallis quis aliquam mauris suscipit.
                </p>
            </div>
            <div class="pin">
                <img src="http://loremflickr.com/640/480/germany" />
                <p>
                    4 Donec a fermentum nisi. Integer dolor est, commodo ut sagittis vitae, egestas at augue.
                </p>
            </div>
            <div class="pin">
                <img src="http://dummyimage.com/480x4:3" />
                <p>
                    5 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed feugiat consectetur pellentesque. Nam ac elit risus, ac blandit dui. Duis rutrum porta tortor ut convallis. Duis rutrum porta tortor ut convallis.
                </p>
            </div>
            <div class="pin">
                <img src="http://dummyimage.com/480x3:4" />
                <p>
                    6 Nullam eget lectus augue. Donec eu sem sit amet ligula faucibus suscipit. Suspendisse rutrum turpis quis nunc convallis quis aliquam mauris suscipit. Duis rutrum porta tortor ut convallis.
                </p>
            </div>
            <div class="pin">
                <img src="http://dummyimage.com/640x21:10" />
                <p>
                    7 Nullam eget lectus augue.
                </p>
            </div>
            <div class="pin">
                <p>
                    8 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed feugiat consectetur pellentesque.
                </p>
            </div>
            <div class="pin">
                <img src="http://dummyimage.com/800x4:3" />
                <p>
                    9 Donec a fermentum nisi. Integer dolor est, commodo ut sagittis vitae, egestas at augue. Suspendisse id nulla ac urna vestibulum mattis. Duis rutrum porta tortor ut convallis.
                </p>
            </div>
            <div class="pin">
                <img src="http://dummyimage.com/900x4:2" />
                <p>
                    10 Donec a fermentum nisi. Integer dolor est, commodo ut sagittis vitae, egestas at augue. Suspendisse id nulla ac urna vestibulum mattis.
                </p>
            </div>
            <div class="pin">
                <img src="http://dummyimage.com/640x5:4" />
                <p>
                    11 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed feugiat consectetur pellentesque. Nam ac elit risus, ac blandit dui. Duis rutrum porta tortor ut convallis.
                </p>
            </div>
            <div class="pin">
                <img src="http://loremflickr.com/1024/768/cool" />
                <p>
                    12 Donec a fermentum nisi. Integer dolor est, commodo ut sagittis vitae, egestas at augue. Suspendisse id nulla ac urna vestibulum mattis.
                </p>
            </div>
            <div class="pin">
                <img src="http://dummyimage.com/800x16:3" />
                <p>
                    13 Donec a fermentum nisi. Integer dolor est, commodo ut sagittis vitae, egestas at augue. Suspendisse id nulla ac urna vestibulum mattis.
                </p>
            </div>
            <div class="pin">
                <img src="http://loremflickr.com/1024/768/vw,golf,variant/all" />
                <p>
                    14 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed feugiat consectetur pellentesque. Nam ac elit risus, ac blandit dui. Duis rutrum porta tortor ut convallis.
                </p>
            </div>
            <div class="pin">
                <img src="http://dummyimage.com/300x4:3" />
                <p>
                    15 Nullam eget lectus augue.
                </p>
            </div>
            <div class="pin">
                <img src="http://dummyimage.com/640x16:9" />
                <p>
                    16 Nullam eget lectus augue.
                </p>
            </div>
        </div>
    </div>
</body>

</html>
```
