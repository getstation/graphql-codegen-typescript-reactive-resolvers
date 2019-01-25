# TypeScript reactive resolvers for GraphQL code generator
> [GraphQL Code Generator](https://github.com/dotansimha/graphql-code-generator) plugin to generate TypeScript typing of [reactive-graphql](https://github.com/mesosphere/reactive-graphql/) resolvers.

## Installation

`npm install graphql-codegen-typescript-reactive-resolvers --save-dev`

## Usage

Run `gql-gen` as usual with this config:

```js
schema: schema.json
overwrite: true
generates:
  ./src/resolvers-types.ts:
    plugins:
      - typescript-common
      - typescript-reactive-resolvers
```

### How does it work

It's almost the same than [typescript-resolvers](https://graphql-code-generator.com/docs/plugins/typescript-resolvers) except that resolvers can return rxjs's Observable.

