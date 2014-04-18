# &lt;instagram-feed&gt;

A [Polymer](http://polymer-project.org) element for displaying an Instgram user's feed.

Somewhat inspired by Addy Osmani's [x-instagram](http://github.com/addyosmani/x-instagram), though a bit different for my needs.

## Usage

1. Import Web Components' polyfill:

```html
<script src="//cdnjs.cloudflare.com/ajax/libs/polymer/0.1.4/platform.js"></script>
```

2. Import custom element:

```html
<link rel="import" href="src/instagram-feed.html">
```

3. Using it:

```html
<instagram-feed userId="USER_ID_WHOSE_FEED_YOU_WANT" accessToken="YOUR_INSTAGRAM_API_ACCESS_TOKEN"><instagram-feed>
```

Additional attribute options:

- count: the number of Instagram images to display; defaults to 8
- imageSize: 'small', 'medium', or 'large'; the size of the Instagram image rendered; defaults to 'small'

```html
<instagram-feed userId="someId" accessToken="someToken" count="10" imageSize="large"><instagram-feed>
```

## Demo

Install dependencies:

1. Install [Node.js](http://nodejs.org/download/)
2. Install [Grunt](http://gruntjs.com/):

```sh
$ npm install -g grunt-cli
```

3. Install Node dependencies:

```sh
$ npm install
```

4. Install bower dependencies:

```sh
$ bower install
```

5. Run a local server:

```sh
$ grunt connect
```

6. Edit the `&lt;instagram-feed&grt;` in `index.html`; provide real `userId` and`accessToken` attribute
values. See [Instagram developer documentation](http://instagram.com/developer/) for more info.

6. Visit `http://localhost:8000` in your web browser.

## License

[MIT License](http://opensource.org/licenses/MIT)
