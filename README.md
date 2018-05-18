# Use resin.io to provision your flogo app on end IoT device

For more information on Flogo, Visit http://flogo.io.

You will learn how to build Flogo applications with the Flogo graphical Web UI.

Here, my simple application is described in the flogo-simple-app.json file

This app is a simple REST Server :

It accepts GET request on /hello/[Your_Name] and then replies with a greetings sentence like 
```
{"Greetings":"Welcome to Project Flogo, [Your_Name]. My name is Flynn !"}
````

## Resin.io instructions

It's easy. Just follow the Getting Started instructions [here](https://docs.resin.io/learn/getting-started/raspberrypi3/nodejs/), and just apply the 2 following changes:
1. In the "Deploy Code" section, here is the repo you need to clone
```
$ git clone https://github.com/ecarlier-tibco/flogo-resin.io.git
```
2. When testing the app using the public device URL, you should add '/hello/[Any_Name]' at the end of the URL
