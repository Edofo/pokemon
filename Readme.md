## Hello, Pokemon

## <a name='TOC'>🐼 Summary</a>

- [Rules](#rules)
- [Overview](#overview)
- [Exercises](#exercises)
- [Credits](#credits)

## <a name='overview'>🦊 Rules</a>

Hi, here are some rules to carry out this project:

- You **MUST** create a git repository named `cx-node-pokemon`
- You **MUST** create a file called `.author` with your firstname and lastname followed by a newline.

```sh
~/pokemon ❯❯❯ cat -e .author
Majdi Toumi$
```

> Of course, you can talk about the subject with other developers, peer-learning is
> the key to be a better developer. Don't hesitate to ask questions or help people on Teams.

> Don't forget, there is no useless question :-)

- You **MUST** return all exercises before Friday November, 27 at 16:00
- You **MUST** add `pu-erh` user as a collaborator.
- YOU **MUST** define all functions signature by yourself :)

## <a name='overview'>🐱 Overview</a>

The purpose of theses exercises is simple : create a simple API server about Pokemons.

## <a name='steps'>🐨 Steps</a>

### 01 Duplicate the pokedex

You have to create a file named `pokedex-YYYYMMDD.json` which is copy of the file [**pokedex.json**](./pokedex.json)

> Replace YYYY by the current year, MM the current month and DD the day

Ex:
```sh
~/pokemon ❯❯❯ ls
server.js pokedex.json pokedex-20201127.json
```

### 02 Bootsrap an API

Create a node js server that listent on a port define in args

Ex:
```sh
~/pokemon ❯❯❯ node server.js 4242
Server is listening on http://localhost:4242
```

### 03 CRUD Pokemon

We'll allow to Create (POST), Update (PUT) or Delete a pokemon. But also to Read (GET) all or one pokemon,
Our application should have the following routes:

- `GET /pokemons` - this should respond with a list of all pokemons.
- `GET /pokemons/:id` - this route should display a single pokemon's found on your daily pokedex.json
- `POST /items` - this route should add a new pokemon on your pokedex.
- `DELETE /items/:id` - this route should allow you to delete a specific pokemon

Ex of one pokemon from Pokedex :

```json
    "id": 1,
    "name": {
      "english": "Bulbasaur",
      "japanese": "フシギダネ",
      "chinese": "妙蛙种子",
      "french": "Bulbizarre"
    },
    "type": [
      "Grass",
      "Poison"
    ],
    "base": {
      "HP": 45,
      "Attack": 49,
      "Defense": 49,
      "Sp. Attack": 65,
      "Sp. Defense": 65,
      "Speed": 45
    }
    ...
```

> For POST you must fill the fields: `name` and `type`

### 04 BONUS // Query parameters

Update the the `GET /pokemons` routes to allow you to search specifics pokemon using query parameters
- name
- type 

## <a name='credits'>🐵 Credits</a>

Craft with :heart: in **Paris**.
