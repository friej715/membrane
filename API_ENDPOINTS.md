`POST /register` - register a new author

`GET /authors` - get all the authors

`GET /promptsets` - see all promptsets

`GET /promptsets/{author}` - get an author's promptset

`POST /promptsets` - add a promptset


```GET /users``` - get all the users

```POST /users``` - add a user

```GET /users/check``` - lookup user (for frontend cookie checking)

```GET /users/{userId}``` - get one particular user

```GET /users/{userId}/prompts``` - get all prompts submitted by a particular user


```GET /responses``` - get all the responses

```POST /responses``` - add a response

```DELETE /responses/{responseId}``` - delete a response

```GET /responses/{responseId}``` - get one particular response

```GET /responses/{responseId}/prompts``` - get all the children of a given response.

`PUT /slug/{slug}` - update a response

```GET /responses/{responseId}/prompts/answered``` - get all the children of a given response *that also have responses as children.* E.g., if you want to get all prompts branching off a response, but limit those prompts only to ones that have child responses in response. Useful for frontend development, so users don't see the whole mass of prompts posted on a response.

`GET /responses/{responseId}/prompts/anchors` - get all the prompts that are answered+anchors

`GET /responses/{responseId}/ancestor` - get an anchor ancestor for a given response

```GET /prompts``` - get all the prompts

```POST /prompts``` - add a prompt

```POST /prompts/{promptId}``` - update prompt anchor state

```DELETE /prompts/{promptId}``` - delete a prompt

```GET /prompts/{promptId}``` - get one particular prompt

```GET /prompts/{promptId}/responses``` - get all the children of a given prompt.

```GET /notifications``` - get all notifications

```POST /notifications/user/``` - get all notifications for a given user (intended for frontend use--posts cookie)

```POST /notifications/user/read``` - mark all notifications for a given user as read

```POST /notifications``` - add a notification