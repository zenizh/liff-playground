# LIFF Playground

This is a web application that allows you to try out the basic features of the LINE Front-end Framework (LIFF). For example, you can deploy the following playground to your server.

* [LIFF Playground](https://liff-playground.netlify.app)

## Table of contents

* [Preparation](#preparation)
  1. [Get a LIFF ID](#1-get-a-liff-id)
  1. [Set the LIFF ID](#2-set-the-liff-id)
* [Usage](#usage)
  * [Run on local](#run-on-local)
  * [Deploy to a server](#deploy-to-a-server)

## Preparation

### 1. Get a LIFF ID

To start the LIFF Playground, you need to obtain a LIFF ID from the [LINE Developers Console](https://developers.line.biz/console/). Follow the steps below to obtain a LIFF ID.

* [Create a channel](https://developers.line.biz/en/docs/liff/getting-started/)
* [Adding a LIFF app to your channel](https://developers.line.biz/en/docs/liff/registering-liff-apps/)

### 2. Set the LIFF ID

Set the LIFF ID obtained in the above procedure as an environment variable. Open `.env` and set the LIFF ID.

````
REACT_APP_LIFF_ID="Your LIFF ID"
````

## Usage

This section shows two ways to run it on local and deploy it on a server.

### Run on local

To run the LIFF Playground on local, first install the dependent packages. Then run the application.

```bash
$ npm install
$ npm start
```

This will start it up. When you access the URL shown in the terminal, you can see the LIFF Playground.

### Deploy to a server

This section shows an example of deploying LIFF Playground to [Netlify](https://www.netlify.com/). You can deploy it from the Deploy button below.

[![](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/zenizh/liff-playground)

After executing the above, the LIFF Playground will be deployed on Netlify. The next step is to get the URL of the deployed page.

Then register this URL on the [LINE Developers Console](https://developers.line.biz/console/). Register this URL as the `Endpoint URL` in the LIFF app settings page. See [Adding a LIFF app to your channel](https://developers.line.biz/en/docs/liff/registering-liff-apps/) for instructions on how to register.

That's it! The LIFF Playground will appear when you access the deployed URL. You can confirm that LINE Login and other features work properly.