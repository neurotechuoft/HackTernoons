# NeurotechUofTFrontendTutorial

### Overview
This is a frontend tutorial meant for complete beginners. In this project, we will first make a basic webpage using HTML / CSS to plot data from a CSV file. The sample data in this repository are responses from an EEG.

After we have the basic web-page built, we will transition the project into a ReactJS app. Here, we will be able to connect the Muse EEG headset to the app, and plot **actual** data from your brain, in real time!

#### Part 1: HTML Programming
Every HTML page starts off with the initial structure below.
```html
<!DOCTYPE html>
<html>
  <head>
  </head>
  <body>
  </body>
</html>
```
There is one large ```<html>``` tag, with a  ```<head>``` and a ```<body>``` tag nested inside. We also call tags "HTML elements".


The ```<head>``` and ```<body>``` tags split up the region of the webpage, as shown below.

<a ><img src="./HTMLStructure.png" width="240" height="180" /></a>

All HTML elements placed inside the ```<body>``` tag will be shown in the CONTENT region shown in the above photo. In this tutorial, we will store everything in the  ```<body>``` tag.

We'll start by adding a header to the page.
