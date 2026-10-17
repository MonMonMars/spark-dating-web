# spark-dating-web

Public tap-through demo of Spark. The page is a phone frame with Discover, Map, Matches, Spark+, and Profile. Sample people are built into the page, so the demo still runs when the network call fails. When the call succeeds, the deck and map use live demo data.

## Live site

https://monmonmars.github.io/spark-dating-web/

GitHub Pages serves this repository as a static site. `index.html` is the site root.

## API

Deck, map people, and demo events come from the Spark Supabase project:

`https://zvcxbrdhikeizyaumtsg.supabase.co/functions/v1/demo-data`

The page GETs that function to load the deck, people, and chats, and POSTs demo events to the same function. A failed request leaves the built-in sample data in place.

## License

MIT — see [LICENSE](./LICENSE).
