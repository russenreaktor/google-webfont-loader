# google-webfont-loader

See the [component page](http://russenreaktor.github.io/google-webfont-loader) for more information.


## Getting Started
Add it via bower
  "dependencies": {
    "google-webfont-loader": "git@github.com:russenreaktor/google-webfont-loader.git#~0.0.2"
  }
  

## Using
 <google-webfont-loader fonts="Droid Sans,Droid Serif"></google-webfont-loader>

    document.querySelector('google-webfont-loader').addEventListener('fonts-active', function(e) {
        console.log('fonts-active', e.detail.fonts);
    });
    

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install


## Playing With Your Element

If you wish to work on your element in isolation, we recommend that you use
[Polyserve](https://github.com/PolymerLabs/polyserve) to keep your element's
bower dependencies in line. You can install it via:

    npm install -g polyserve

And you can run it via:

    polyserve

Once running, you can preview your element at
`http://localhost:8080/components/google-webfont-loader/`, where `google-webfont-loader` is the name of the directory containing it.


## Testing Your Element

Simply navigate to the `/test` directory of your element to run its tests. If
you are using Polyserve: `http://localhost:8080/components/google-webfont-loader/test/`

### web-component-tester

The tests are compatible with [web-component-tester](https://github.com/Polymer/web-component-tester).
Install it via:

    npm install -g web-component-tester

Then, you can run your tests on _all_ of your local browsers via:

    wct

#### WCT Tips

`wct -l chrome` will only run tests in chrome.

`wct -p` will keep the browsers alive after test runs (refresh to re-run).

`wct test/some-file.html` will test only the files you specify.
