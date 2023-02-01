---
title: Convert Variable Font OTF to WOFF2
---

**If you are using online font generators they will break variable fonts as they are designed for static font faces. They will remove all except the default font face.**

{% include youtube.html id="2BxdUmEvqFA" %}

Create a folder on your desktop. Open your terminal.

Type CD and drag your folder. That way you don't need to type your path.

## Build

```
git <strong>clone</strong> --recursive https://github.com/google/woff2.git
cd woff2
make clean all
```

## Run

```
./woff2_compress path_to_font/myfont.ttf;
```

You will get a converted .woff2 file next to your file.

## GitHub Code

https://github.com/google/woff2
