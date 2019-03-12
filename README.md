# Overview
'chatux' is a library that allows you to easily create chat windows on your PC or mobile

It is licensed under [MIT](https://opensource.org/licenses/MIT) license.

###  What is '**chatux**' like?
It is an independent and lightweight chat user interface (chat UI) library for javascript.

- You can create pages for chat agents and chat bots that support both smartphones and PCs.
- For PC, show chat in a window that does not disturb existing content
- For mobile dvices like smartphones and tablets, chat UI will be overlaid on existing pages to avoid disturbing existing content

<img src="https://riversun.github.io/chatux/guide.png">

# DEMO
https://riversun.github.io/chatux/

<img src="https://riversun.github.io/chatux/chatux_qr.png">

**How to play demo.**

This demo is simple echo chat.
But a few command available.If you write "show buttons", you can see action buttons in chat.
Or you write "show image", you can see image in chat.

# Quick start

Check this example.

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <title>chatux example</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
</head>
<body style="padding:0px;margin:0px;">
<div style="padding:40px">
    <h1>chatux example</h1>
    <p> Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
</div>
<script src="https://riversun.github.io/chatux/chatux.min.js"></script>
<script>

    const chatux = new ChatUx();

    const opt = {
        api: {
            //URL of chat server
            endpoint: 'https://script.google.com/macros/s/AKfycbwpf8iZfGXkJD6K__oCVQYF35HLBQjYxmKP0Ifrpe_piK4By4rh/exec',
            //HTTP METHOD
            method: 'GET',
            //DATA TYPE
            dataType: 'jsonp'
        },
        window: {
            title: 'My chat',
            infoUrl: 'https://github.com/riversun/chatux'
        }
    };

    //initialize
    chatux.init(opt);
    chatux.start(true);

</script>
</body>
</html>

```

**Show on PC**

<img src="https://riversun.github.io/chatux/onpc.png">

**Show on mobile**

<img src="https://riversun.github.io/chatux/onmobile.png">

## install

### using npm

```
npm install chatux --save
```

### using with script tag

```
<script src="https://riversun.github.io/chatux/chatux.min.js"></script>
```
