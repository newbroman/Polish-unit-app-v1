# Polish Food Master

A quiz on the Polish grammar of quantities and units: pick the correct form of a unit (kilogram, bottle, bag and so on) for the number shown.

**Live app:** https://newbroman.github.io/Polish-unit-app-v1/

## Features

- Each question gives a Polish phrase with a blank, such as a number word followed by a unit, and an English translation of the quantity.
- Four answer buttons: nominative singular, nominative plural, genitive plural and genitive singular forms of the unit.
- Quantities of 1 to 9, plus 0.5 (pół) and 1.5 (półtora / półtorej), with the number word matched to the unit's gender.
- Unit and gender colour coding (masculine, feminine, neuter), and an explanation after each answer.
- About 100 items across food (fruit, vegetables, meat, drinks and more), building materials, finishing, hardware, electrical items and tools.
- Pronunciation of each phrase through speech synthesis, a streak counter, and a mastery bar (an item is mastered after 5 correct answers).
- Progress is saved automatically in the browser, with a reset button; English and Polish interface text.

## Using it

Open the live app in a browser and press Start Training; the Rules button reopens the instructions. Audio uses the browser's speech synthesis, so a Polish (pl-PL) voice is needed to hear the phrases. It is a plain web page with no manifest or service worker, so it is not installable and needs a connection to load.

## Project structure

- `index.html` - the app: layout, styles and quiz logic.
- `data.js` - the unit table (all case forms, gender, English name) and the item list with categories and permitted units.

## Development

No build step. From the repository folder run:

```
python3 -m http.server
```

then open http://localhost:8000. To add items or units, edit `data.js`.

Built by Martin Hollingham.
