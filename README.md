# chess.com.bruno

A collection of [Bruno][bruno.com] requests for the [Chess.com][chess.com] public API

## Usage

Since these requests hit the Chess.com public API, no prior setup or authorization is needed

Simply download and open this repo in Bruno and select the `chess.com` environment to set all global variables used by the requests to the correct values

#### Environment Variables

The following is a list of variables used by most of the requests in this project. Not all varaibles are used by all collections

1. `baseUrl`
- The common url path for all requests
- Should always be set to `https://api.chess.com/pub`

2. `username`
- Used by requests in the `player` collection to determine which user to request data for

3. `clubId`
- Used by requests in the `club` collection to determine which club to request data for

4. `tournamentId`
- Used by requests in the `tournaments` collection to determine which tournament to request data for

5. `matchId`
- Used by requests in the `teamMatch` collection to determine which teamMatch to request data for
- Requests for live matches in the same collection also use this variable

6. `countryCode`
- Used by requests in the `countries` collection to determine which country to request data for
- See the country section of the Chess.com [public API docs][chess.com-public-api-docs] for more information on the available country codes

#### Request Variables

Apart from the above, certain requests will also use there own request-scoped variables

Check the `Vars` tab in Bruno to see if the requests being used need additional configuration

#### Quick Tips

For requests that require the a month value to be passed to the request through varaibles (for example, the `player/pgnArchive` request), format any single digit month as `MM` and wrap in `''` characters to pass the correct value to the request

## Useful Links

Check out the full Chess.com public API docs [here][chess.com-public-api-docs]

If you elitist and prefer Postman 😆, check out the official Chess.com Postman collections [here][chess.com-postman-schema]

## Licence

Haha, there is no licence. Use this project in whatever morally correct way you'd like 😎

## Contributing

Please feel free to file any issues or suggestions in the projects' [Github repo][github-repo]

[bruno.com]: https://www.usebruno.com
[chess.com]: https://www.chess.com
[chess.com-public-api-docs]: https://www.chess.com/news/view/published-data-api
[chess.com-postman-schema]: https://www.chess.com/postman/collection-dev.json
[github-repo]: https://github.com/taennan/chess.com.bruno
