# svelte-intro.js
![npm](https://img.shields.io/npm/v/svelte-intro.js) ![NPM](https://img.shields.io/npm/l/svelte-intro.js) ![GitHub top language](https://img.shields.io/github/languages/top/etuncay/svelte-intro.js) ![npm](https://img.shields.io/npm/dm/svelte-intro.js)


### Installation

```sh
$ npm i svelte-intro.js --save-dev
```

### Example 1
Hello World!

```html
<script >
	import IntroJs from "$lib/intro-js.svelte";

  <IntroJs>
    <div data-title="Welcome!" data-intro="Hello World! 👋" class="card-demo">
        <div class="card shadow--md">
          <div class="card__image" data-intro="Intro.js can highlight on elements">
            <img src="https://fakeimg.pl/300/" alt="Image alt text" title="Logo Title Text 1" />
          </div>
          <div class="card__body" data-title="Farewell!" data-intro="And this is the last step!">
            <h4>Quaco Lighthouse</h4>
            <small>
              The Quaco Head Lighthouse is a well maintained lighthouse close to St.
              Martins. It is a short, beautiful walk to the lighthouse along the
              seashore.
            </small>
          </div>
        </div>
      </div>
  </IntroJs>
```


### Example 2
JSON configuration
```html
<script >
	import IntroJs from "$lib/intro-js.svelte";

      
    let options = {
          steps: [{
              title: 'Welcome',
              intro: 'Hello World! 👋json'
          },
          {
              selector: '.card-demo',
              intro: 'This step focuses on an image json'
          },
          {
              title: 'Farewell!',           
              selector: '.card__image',
              intro: 'And this is our final step! json'
          }]
        };
  </script>
  <IntroJs {options}>
    <div data-title="Welcome!" data-intro="Hello World! 👋" class="card-demo">
        <div class="card shadow--md">
          <div class="card__image" data-intro="Intro.js can highlight on elements">
            <img src="https://fakeimg.pl/300/" alt="Image alt text" title="Logo Title Text 1" />
          </div>
          <div class="card__body" data-title="Farewell!" data-intro="And this is the last step!">
            <h4>Quaco Lighthouse</h4>
            <small>
              The Quaco Head Lighthouse is a well maintained lighthouse close to St.
              Martins. It is a short, beautiful walk to the lighthouse along the
              seashore.
            </small>
          </div>
        </div>
      </div>
  </IntroJs>

```

For introjs documentation and more examples
You can visit [introjs](https://introjs.com/docs/)


### Author
Emrullah TUNCAY

License
----

MIT
