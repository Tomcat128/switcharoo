# SWITCHAROO

Fetches current switch games on sale from the nintendo store. Also looks up the metacritic score. The final result
will be a basic data table, sorted by metacritic rating.
Works for european :video_game: store only.

![example](example.png "an example screenshot")

## Setup

Fetching the rating from metacritic requires a rapid api key. Therefore you'll need a api key from
[Rapid API](https://rapidapi.com/). :runner:

You can pass the key along by setting the environment variable `API_KEY_METACRITIC`, or define the key in an `.env`
file in the project's root, like so:
```
PORT=3000
API_KEY_METACRITIC=${put_your_rapid_api_key_here}
``` 

Then simply install and run it:

```bash
npm install
npm run
```

Since that's probably the first time starting the application, you'll need to open you browser and navigate to the fetch
endpoint at [http://localhost:3000/fetch](http://localhost:3000/fetch). This may take a while. If everything goes well
you'll be notified with the amount of games found. You'll also find a games.json file at [data/games.json](data/games.json).

At [localhost:3000](http://localhost:3000) you should now find something similar to the sceenshot above. :see_no_evil: