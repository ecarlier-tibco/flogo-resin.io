# Use resin.io to provision your flogo app on end IoT device

### IoT Simplified

Use **Project Flogo** to develop IoT Edge application with no code using the Graphical development web UI, and then **resin.io** to push your code, and have it deploy automatically to a float of devices

## Flogo instructions

For more information on Flogo, Visit http://flogo.io.

You will learn how to build Flogo applications with the Flogo graphical Web UI.
Once you've developed an application using Flogo Web UI, you can export it as a JSON file, and use this JSON file to version control your application with git.

Here, my simple application was exported and is described in the flogo-simple-app.json file

This app is a simple REST Server accepting GET requests on /hello/[Any_Name] path and replying with a greetings sentence in a JSON payload: 
```
{"Greetings":"Welcome to Project Flogo, [Any_Name]. My name is Flynn !"}
````

## Resin.io instructions

It's easy. Just follow the Getting Started instructions [here](https://docs.resin.io/learn/getting-started/raspberrypi3/nodejs/), and just apply the 2 following changes:
1. In the "Deploy Code" section, here is the repo you need to clone
```
$ git clone https://github.com/ecarlier-tibco/flogo-resin.io.git
```
2. When testing the app using the public device URL, you should add '/hello/[Any_Name]' at the end of the URL
