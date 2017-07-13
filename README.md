# bem-twig-extension
Twig function that inserts static classes into Pattern Lab but adds them to the attributes object in Drupal

## Usage

#### Simple block name:
`<h1{{ bem('title') }}>`

This creates:

`<h1 class="title">`

#### Block with modifiers (array allowing multiple modifiers):
`<h1{{ bem('title', ({1: 'small', 2: 'red'})) }}>`

This creates:

`<h1 class="title title--small title--red">`

#### Element with modifiers and blockname:
`<h1{{ bem('title', ({1: 'small', 2: 'red'}), 'card') }}>`

This creates:

`<h1 class="card__title card__title--small card__title--red">`
