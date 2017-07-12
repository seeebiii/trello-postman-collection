# trello-postman-collection
A Postman collection for Trello REST Api. Collection is saved in v2.


## Install
1. Download [the collection file](Trello.postman_collection) and save it on your computer.
2. Follow [these instructions](https://www.getpostman.com/docs/postman/collections/data_formats) to include it into your Postman.
3. Consider the notes below and use it :)


## Notes
- You have to create an environment in Postman including at least the key `host`. This should always have the value `https://api.trello.com/1`. Take a look [here on how to create environments](https://www.getpostman.com/docs/postman/environments_and_globals/manage_environments).
- Since Trello is using OAuth 1.0a, for a request you need to select *OAuth 1.0* within the *Authorization* tab in Postman. Take a look [here](https://www.getpostman.com/docs/postman/sending_api_requests/authorization). Therefore in this Trello collection, the following keys are assumed to be available in the environment configuration: `consumer_key`, `consumer_secret`, `token`, `token_secret`. Take a look [here and get your Trello API keys](https://trello.com/app-key).


## Supported Endpoints

|Method|Path|
|------|-----|
|GET|/boards|
|GET|/boards/:id|
|GET|/boards/:id/actions|
|GET|/boards/:id/cards|
|GET|/boards/:id/labels|
|GET|/boards/:id/lists|
|GET|/boards/:id/members|
|GET|/boards/:id/organization|
|PUT|/boards/:id|
|POST|/boards|
| | |
|GET|/cards/:id|
|GET|/cards/:id/actions|
|GET|/cards/:id/attachments|
|GET|/cards/:id/board|
|GET|/cards/:id/checklists|
|GET|/cards/:id/list|
|GET|/cards/:id/members|
|GET|/cards/:id/stickers|
|PUT|/cards/:id|
|PUT|/cards/:id/desc|
|POST|/cards|
|DELETE|/cards/:id|
| | |
|GET|/lists/:id|
|GET|/lists/:id/actions|
|GET|/lists/:id/board|
|GET|/lists/:id/cards|
|PUT|/lists/:id|
|POST|/lists|
| | |
|GET|/members/me|
|GET|/members/:id/actions|
|GET|/members/:id/boards|
|GET|/members/:id/cards|
|GET|/members/:id/notifications|
|GET|/members/:id/organizations|
|GET|/members/:id/tokens|
| | |
|GET|/tokens/:token|
|GET|/tokens/:token/webhooks|
| | |
|GET|/webhooks/:id|
|PUT|/webhooks|
|DELETE|/webhooks/:id|


## License
MIT License

Copyright (c) 2017 [Sebastian Hesse](https://www.sebastianhesse.de)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
