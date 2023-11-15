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