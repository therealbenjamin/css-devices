#CSS Devices

Readymade and responsive desktop, tablet, and phones in pure SASS baby!

Since everything is done in SASS, you can fine-tune the solution to your needs, breakpoints, color scheme, etc. Just change the variables to rock and roll.

##Installation

Okay, so you're ready to rock an roll? There's two options to install this thing:

###Bower

```bower install css-devices```

Then include the stylesheet...

```<link rel="stylesheet" type="text/css" href="bower_components/css-devices/css/css-devices.min.css">```

###Download

[Minified CSS](https://raw.githubusercontent.com/gustodev/css-devices/master/css/css-devices.min.css) and then include the stylesheet...

```<link rel="stylesheet" type="text/css" href="path/to/css-devices.min.css">```

##Devices

Currently there are five visual devices, two of which come in both portrait and landscape orientation.

There are buttons which are color coordinated via classes generated by SASS.  You can add as many colors as you'd like and these buttons are available for use anywhere in the devices.  In the first example, the browser device, you can see we're using four buttons: three on the left and one on the right.  Feel free to customize these classes to your heart's content by editing the SASS.  We also include inset classes for a slight inset box shadow on any of the color classes.  I think they look nice on the buttons, so I included them here.

###Browser

```
<div class="device browser">
    <div class="header">
        <div class="left">
            <span class="button red inset"></span>
            <span class="button yellow inset"></span>
            <span class="button green inset"></span>
        </div>
        <div class="right">
            <span class="button dark inset"></span>
        </div>
    </div>
    <div class="container" style="background-image: url('path/to/image.png');"></div>
</div>
```

This device has an optional header (which aesthetically you should probably have anyhow).  Just include the background image of what you want inside on the `background-image` of the `.container` div and go to work!

###Mobile

```
<div class="device mobile">
    <div class="top"></div>
    <div class="container" style="background-image: url('path/to/image.png');"></div>
    <div class="home">
        <span class="button dark inset"></span>
    </div>
</div>
```

Same idea here as in the browser above.  Here we have an optional `.top` and an optional `.home` section.  You may also make the device be in landscape mode by adding a `.landscape` class to the `.device` class as such:

```<div class="device mobile landscape">```

###Tablet

```
<div class="device tablet">
    <div class="top"></div>
    <div class="container" style="background-image: url('path/to/image.png');"></div>
    <div class="home">
        <span class="button dark inset"></span>
    </div>
</div>
```

Tablets are done the same as mobiles are and are also therefore landscape via the `.landscape` class.  Keep in mind, you can change the dimensions to whatever you please via SASS.

###Desktop

```
<div class="device desktop">
    <div class="container" style="background-image: url('path/to/image.png');"></div>
    <div class="stand"></div>
</div>
```

This is how you include a desktop.  They also include a sexy little stand with them.  Again, if you don't want it then remove it (but then it might look like a peculiar-looking tablet).

###Laptop

```
<div class="device laptop">
    <div class="container" style="background-image: url('path/to/image.png');"></div>
    <div class="body"></div>
</div>
```

In much the same way as desktops, laptops are done.  The only key difference is that the `.stand` class from desktops is called `.body` for obvious reasons.

##Examples

To view all the examples, please go to the following link: [http://gustodev.github.io/css-devices/](http://gustodev.github.io/css-devices/).

##Support

If you need any help, please feel free to contact me at [patrick@gusto.is](mailto:patrick@gusto.is).  If you'd like to add, change, or improve to CSS Devices, then fork and PR to your heart's content!

Much <3 from [Gusto](http://gusto.is)!
