# *ZZR*'s Personal Page

[![Build Status](https://travis-ci.org/pages-themes/cayman.svg?branch=master)](https://travis-ci.org/pages-themes/cayman) [![Gem Version](https://badge.fury.io/rb/jekyll-theme-cayman.svg)](https://badge.fury.io/rb/jekyll-theme-cayman)

*GitHub page theme: [preview the theme to see what it looks like](http://pages-themes.github.io/cayman), or even [use it today](#usage).*

![Thumbnail of Cayman](thumbnail.png)

## Self-Descriptions

Me, *Zhang Zirui*, borned in *Luzhou* City, *Sichuan*, China on November 28^th^, 2006. Now in the Luzhou Maple Leaf Jiade International School. I've studied programming for only 1.5 year by now (today May 22^nd^, 2021). When I was a pupil, I was the best in computer using, even had to design PowerPoint for a few subjects. It was the day October 22^nd^ in 2019, I saw a few large text on my Computer Technology book ---- "**Python**". From then on, I fell into Python coding. Sometimes I was upset just because of a unsolved bug in my programs.

In the middle school, I challenged myself, I got the first place in the *Sichuan* Python Coding Game. Of course, I'm not professional in coding, I never want to code as a job, either. So it's unnecessary for me to learn a language so well, so I learned C/C++, now I'm going to learn Java a little. Even though coding isn't my dream job, but my dream is that one day I can publish a useful open-source project. To improve my C coding skill, I'm reading *Homemade Operating System in 30 Days* by Hidemi Kawai. I want to be friends with anyone else who likes coding.

## Coding

### Languages I Can Code

So far, I've studied 3 coding languages and I'm studying another. Here are them:

1. Python 3

```python

from django.shortcut import render

from django.models import Model, CharField

class FileModel(Model):

    filename = CharField(max_length=50)

    url = CharField(max_length=150)

    class Meta:

        verbose_name = 'File Model'

        verbose_name_plural = 'File Models'

# Code above: [CPython 3.7.4] Django

```

2. C/C++

```cpp

#include <QWidgets/QMainWindow>

#include <QWidgets/QWidget>

class MainWindow: public QMainWindow

{

    Q_WIDGET

    void setupUi(QWidget* w)

    {

        // TODO

    }

}

// Code above: [C++] Qt open-source

```

3. Assembly

```nasm

        MOV      AX,0x0820

        MOV      ES, AX

        MOV      CH,0

        MOV      DH,0

        MOV      CL,2

readloop:

        MOV      SI,0

retry:

        MOV      AH,0x02

        MOV      AL,1

        MOV      BX,0

        MOV      DL,0x00

        INT      0x13    ; Call disk BIOS

        JNC      next

        ADD      SI,1

        CMP      SI,5

        JAE      error

        MOV      AH,0x00

        MOV      DL,0x00

        INT      0x13   ; Reset the driver

        JMP      retry

next:

        MOV      AX, ES

        ADD      AX,0x0020

        MOV      ES, AX

        ADD      CL,1

        CMP      CL,18

        JBE      readloop

        MOV      CL,1

        ADD      DH,1

        CMP      DH,2

        JB       readloop

        MOV      DH,0

        ADD      CH,1

        CMP      CH, CYLS

        JB       readloop

; Code above: [ASM] read disk

```

Studying: Java

```java

package com.example.myapp

import android.app.Activity;

import android.os.Bundle;

import per.study.myapp.R;

public class MainActivity extends Activity {

    @Override

    protected void onCreate(Bundle savedInstanceState) 

    {

    super.onCreate(savedInstanceState);

    setContentView(R.layout.activity_main);

    intentFilter = new IntentFilter();

        intentFilter.addAction("android.net.conn.CONNECTIVITY CHANGE");

                networkChangeReceiver = new NetworkChangeReceiver();

                registerReceiver(networkChangeReceiver, intentFilter);

            }

            @Override

            protected void onDestroy() {

                super.onDestroy();

                unregisterReceiver(networkChangeReceiver);

            }

            class NetworkChangeReceiver extends BroadcastReceiver {

                @Override

                public void onReceive(Context context, Intent intent) {

                    Toast.makeText(context, "network changes", Toast.LENGTH SHORT).show();

                }

            }

}

```

To program better, I also looked through documents of other data formatting.

```html

<!DOCTYPE HTML>

<!-- HTML -->

<html>

<head>

    <title>ZZR's page</title>

    <meta charset="UTF-8">

</head>

<body>

<script type="text/javascript">

    function callback()

    {

        alert("Hello, world");

    }

</script>

</body>

</html>

```

```xml

<?xml version="1.0">

<!-- XML -->

<rootElement>

    <level2 attr="value">

        <!-- TODO -->

    </level2>

</rootElement>

```

```json

// JSON

data {

    key: "word"

}

```

```batch

:: BATCH

cd X:\compile\pro\

gcc -o pro.exe pro.c including.c

pro

```

### Stylesheet

If you'd like to add your own custom styles:

1. Create a file called `/assets/css/style.scss` in your site

2. Add the following content to the top of the file, e
