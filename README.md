# Funny Text Plugin

<img src='https://s3.amazonaws.com/after-school-assets/cat-typing.gif' hspace="10" align="right" width="300px">

Your job is to set up the [Funny Text jQuery Plugin](https://github.com/alvarotrigo/funnyText.js) to create an awesome hover effect over text on your website.

## Let's Get Started

### Step 1:

Click `Open` at the top of this page to bring this lesson down so you can edit files in Nitrous.

<img src="https://s3.amazonaws.com/after-school-assets/new-open-in-nitrous.png">

### Step 2:

Open `index.html` in the browser by running in terminal `python -m SimpleHTTPServer 3000`. 

Once you have the server running, select `preview` and then `port 3000`.

<img src="https://s3.amazonaws.com/after-school-assets/nitrous-preview.png" alt="nitrous preview">


### Step 3:

You're going to code your solution in both `index.html` and `js/script.js`. Go ahead and open both files in the Nitrous text editor. We went ahead and added the files necessary for FunnyText to work. You can find the css file in [`css/jQuery-funny-text.css`](https://github.com/alvarotrigo/funnyText.js/blob/master/jquery.funnyText.css) and the jQuery in [`js/jQuery.funnyText.js`](https://github.com/alvarotrigo/funnyText.js/blob/master/jquery.funnyText.js).


### Step 4:

Take a look at `index.html` in the browser. It should be completely blank.

### Step 5:

The first thing you need to do is correctly link both `js/script.js` and `js/jquery.funnyText.js` to `index.html`. In `index.html`, we already linked to the main jQuery library. You can use that link (located right above the closing body tag) as a template to figure out how to link these two files.

### Step 6:

Next, you need to put some text on the website. Without text, we can't use the plugin. Go ahead and put some text in `index.html`. You'll want to make sure you define an ID or class on the tags. You can write your own text, or use copy and paste this HTML below:

```html
<h1 id="funny"> HEY GUYZ</h1>
```

Go ahead and save the changes to `index.html` and refresh in the browser to make sure the text appears


### Step 7:

Next, you need to use the plugin, and write some code in `js/script.js`. You'll use the ID or class you defined on your HTMl tag as your jQuery selector and call the `.funnyText` method on that. Your code will look something like this:

```js
$(document).ready(function() {
    $('#funny').funnyText();
});
```

Don't forget that you need the document ready to surround your code. Save the changes and refresh in the broswer. Hover your mouse over your text and watch the animations!


### Step 8: 

If you want to get fancy and code your specific animations, you can use this guideline to play around:

```js
$(document).ready(function() {
/////modify the code here
    $('#funny').funnyText({
        speed: 700,
        borderColor: 'black',
        activeColor: 'white',
        color: 'black',
        fontSize: '7em',
        direction: 'both'
    });
//////
});
```

Don't forget, you only need one document ready per file, so you'll be modifying the text in the middle. We've marked it with lots of `/////` for you!

## Done and Done

Lastly, you need to enter in terminal in Nitrous `learn submit`. This command will push your work to GitHub and mark this lesson as complete in Learn!

## Share Share Share!
Show of your work by taking a screenshot of your filled treasure box or code and share with **\#flatironcodeclub**

## Reminder 

Don't forget to shut down your server by hitting `control` and `c` before you move on to other material!