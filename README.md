# HackerNews-Clone

## Using GraphQL, Apollo, and React

built a simple clone of Hackernews. Here’s a list of the features the app will have:

+ Display a list of links
+ Add a new list with name and link

## Technologies for building the app:

# Frontend:

React: Frontend framework for building user interfaces
Apollo Client 2.1: Production-ready, caching GraphQL client

# Backend:

graphql-yoga: Fully-featured GraphQL Server with focus on easy setup, performance & great developer experience
Prisma: Open-source GraphQL API layer that turns your database into a GraphQL API


## How to use

### 1. Clone repository

```sh
git clone git@github.com:yoonmikim/HackerNews-Clone.git
```

### 2. Install dependencies & Deploy the Prisma database API

To install the Prisma CLI globally with Yarn, use the following command:
```sh
yarn global add prisma
```

Also, run the following commands:
```sh
cd react-apollo/server
yarn install
prisma deploy
```

Then, follow these steps in the interactive CLI wizard:

1. Select **Demo server**
1. **Authenticate** with Prisma Cloud in your browser (if necessary)
1. Back in your terminal, **confirm all suggested values**

### 3. Start the server

To start the server, all you need to do is execute the `start` script by running the following command inside the `server` directory:

```sh
yarn start
```

> **Note**: If you want to interact with the GraphQL API of the server inside a [GraphQL Playground](https://github.com/prisma/graphql-playground), you can navigate to [http://localhost:4000](http://localhost:4000).

### 4. Run the app

Now that the server is running, you can start the React app as well. The commands need to be run in a new terminal tab/window inside the root directory `react-apollo` (because the current tab is blocked by the process running the server):

```sh
yarn install
yarn start
```

You can now open your browser and use the app on [http://localhost:3000](http://localhost:3000).
