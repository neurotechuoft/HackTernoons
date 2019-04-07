# Introduction to HTML, CSS, and JavaScript

### Overview
This is a frontend tutorial meant for complete beginners. In this project, we will first make a basic webpage using HTML / CSS to display EEG brainwave data from a CSV file.

#### Part 1: HTML Programming
Create a new folder, and then create a file inside called ```index.html```. Every HTML page starts off with the initial structure below.
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

All HTML elements placed inside the ```<body>``` tag will be shown in the CONTENT region.

For example, let's add a ```<p>``` element inside the ```<body>``` tag, like so:

```html
<body>
  <p>
    Hello world!
  </p>
</body>
```

This should give us a plain webpage that prints "Hello world!" in the CONTENT region. Great!

Now we will insert the following HTML element inside the ```<body>```  tag

```html
<canvas id="chart" width="1000" height="200"></canvas>
```

Here we've made a  ```<canvas>``` element that has a width of 1000 pixels, and a height of 200 pixels. You can think of this element as a blank canvas on the webpage, which we can draw on using JavaScript (our next step)

Now download the following files, and place them in your project folder:  [smoothie.js](https://github.com/neurotechuoft/HackTernoons/blob/master/ReactTutorials/IntroToHTML/smoothie.js),  [EEG_data.jsv](https://github.com/neurotechuoft/HackTernoons/blob/master/ReactTutorials/IntroToHTML/EEG_data.csv), [EEGDataParsedAttention.csv](https://github.com/neurotechuoft/HackTernoons/blob/master/ReactTutorials/IntroToHTML/EEGDataParsedAttention.csv), [EEGDataParsedAttention.jsv](https://github.com/neurotechuoft/HackTernoons/blob/master/ReactTutorials/IntroToHTML/data.json)

EEG_data is a csv file from real EEG data (of confused students, see article at: https://www.kaggle.com/wanghaohan/confused-eeg)! I've taken the 'Attention' column, and transposed it into EEGDataParsedAttention.csv. And then, I stored this into a JavaScript object, and placed that data in data.json.


Take a look at the code at [index.html](https://github.com/neurotechuoft/HackTernoons/blob/master/ReactTutorials/IntroToHTML/index.html). Try copy pasting the JavaScript code from that file into your index.html file, and see what happens!

Try and figure out how that JavaScipt code works. Also, as you can see, I manually parsed the data I needed from EEG_data into the format I wanted for processing. Do you think you can write a JavaScript function to automate this process?

#### Connecting to Python backend
