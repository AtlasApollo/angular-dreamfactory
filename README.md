angular-dreamfactory
====================


The AngularJS DreamFactory module seamlessy integrates the DreamFactory Services Platform(DSP) with an AngularJS application.  Because it is dynamically generated when the application loads your methods and services will always be in sync with your DSP.


The angular-dreamfactory module can be installed by either:

* Cloning or downloading this repo and copying to your project
* using Bower


## Cloning or downloading the repo
This should be self-explanatory.


## Using Bower
First, make sure you have bower installed by opening a command line tool and typing 'bower' at the prompt.
If Bower is installed help text will pop up and you may continue.  If bower is not installed please refer to the [Bower](bower.io) website for help on installing this wonderful tool.

If you have bower or have just finished installing it navigate to your project root and type 'bower install angular-dreamfactory'.  The install should start.  **Pro-tip:** _use the option --save to update your main bower.json file with the angular-dreamfactory dependency._

After the install finishes you are ready to go.


## Including the angular-dreamfactory module

Now that you've installed the module we'll need to include it in th app.  If you have used bower the script should already have been included at the bottom of you index.html file.  If you have not used bower or the script was not included for some reason simply add the following line to where ever you are including your scripts for angular.

```
<script src="_PATH_TO_ANGULAR_DREAMFACTORY_\angular-dreamfactory.js"></script>
```

Now inject angular-dreamfactory into your app (usually in the app.js file).

```javascript
angular.module('MyApp',['ngDreamFactory'])
// The rest of your app
```

The angular-dreamfactory module requires two parameters that we suggest you store as constants in your app definition.  They are your DSP url and your DSP api key.  They should be set like so:

```javascript
.constant('DSP_URL', _YOUR_DSP_URL_HERE_)
.constant('DSP_API_KEY', _YOUR_DSP_API_KEY_HERE_)
```

The first parameters for the constants have to be called exactly 'DSP_URL' and 'DSP_API_KEY' as the angular-dreamfactory module is looking for these to be injected. All together your app definition should resemble the code below:

```javascript
angular.module9'MyApp', ['ngDreamFactory'])
  .constant('DSP_URL', _YOUR_DSP_URL_HERE_)
  .constant('DSP_API_KEY', _YOUR_DSP_API_KEY_HERE_)
// Rest of your app
```





