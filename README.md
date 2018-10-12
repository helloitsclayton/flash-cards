# flash-cards

This is a quick project I put together to see if I could use JavaScript to randomly select vocab words off of a JSON list (`arabic-test.json`) and display them using Reveal.JS

All you'd need to do is drop the contents of this repository directly into an unzipped Reveal.JS directory and you should be good to go. It can be used locally without the need to create a local server if opened using FireFox; I'm unsure about other browsers.

Funcitonality is split between two pages:
* `index.html` in the main directory contains a form which allows users to select parts of speech they wish to practice, whether they'd like to see the English or Arabic first, and the number of flash cards they'd like to have created
* `card-stack/index.html` actually pulls the words from arabic-test.json according to the parameters passed from the above from via the URL; it then randomly selects the number of cards indicated, builds the deck, and displays them
