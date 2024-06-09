
# Storyblok quick starter project

Welcome to this sample project for Nuxt!
This project serves as a quick starter for integrating Storyblok, a headless CMS, into your web development projects.

For starting, you can access to the `portfolio` folder.
In the folder you have some files like:

- `nuxt.config.js`: the configuration with Storyblok API;
- `pages/index.vue`: the initialization of the Storyblok Bridge.

// Install mkcert for creating a valid certificate (Mac OS):

$ brew install mkcert

$ mkcert -install

$ mkcert localhost

// Then install and run the proxy

$ npm install -g local-ssl-proxy

$ local-ssl-proxy --source 3010 --target 3000 --cert localhost.pem --key localhost-key.pem

// https is now running on port 3010 and forwarding requests to http 3000