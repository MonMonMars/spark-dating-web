# spark-dating-web

Public tap-through demo of Spark. The page is a phone frame with Discover, Map, Matches, Spark+, and Profile. Sample people are built into the page, so the demo still runs when the network call fails. When the call succeeds, the deck and map use live demo data.

## Site

https://monmonmars.github.io/spark-dating-web/

`index.html` is the site root. That address serves this demo once GitHub Pages is enabled for the repository (branch `main`, folder `/`, or the Actions workflow in `.github/workflows/pages.yml`).

## API

Deck, map people, and demo events come from the Spark Supabase project:

`https://zvcxbrdhikeizyaumtsg.supabase.co/functions/v1/demo-data`

The page GETs that function to load the deck, people, and chats, and POSTs demo events to the same function. A failed request leaves the built-in sample data in place.

## License

MIT — see [LICENSE](./LICENSE).
