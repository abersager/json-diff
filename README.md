# JSON Diff

Offline browser extension for [https://jsondiff.com/](https://jsondiff.com/)

This fork adds URL parsing functionality to the original JSON Diff tool.

## Motivation

I regularly use [https://jsondiff.com/](https://jsondiff.com/) for comparing JSON documents however it is a website and I have to have internet connectivity always to use it.

So I decided to build a web extension which works offline and easily accessible on a button click.

## Fork-specific Features

This fork extends the original JSON Diff with the following feature:

- **URL Parsing**: URLs can be directly pasted into the input fields and will be parsed into JSON objects with the following structure:
  ```json
  {
    "_protocol": "https",
    "_host": "example.com",
    "_path": "/api/data",
    "param1": "value1",
    "param2": ["value2", "value3"]  // Multiple values for same parameter
  }
  ```
  This makes it easy to compare URL structures, query parameters, and API endpoints.

## Original Features

1. Since this is a offline extension, you download once and run on your laptop whether you are connected to internet or not.
2. Sometimes, the JSON documents we compare may include sensitive information, and it's very important to review the privacy policies and data handling practices of any website before uploading them. However, with the offline extension `JSON Diff`, you can use it without concerns about privacy policies and data handling, as it operates offline.

> **Your data stays in your browser and never leaves your system**.

## Download

To download the extension, visit below links on your respective browsers

Google Chrome: https://chrome.google.com/webstore/detail/json-diff/dmndidoancoefdoobhbmjgignfimpmpj

Mozilla Firefox: https://addons.mozilla.org/en-US/firefox/addon/json-diff/

Below is the extension screenshot

![jsondiff extension](extension.jpg)
