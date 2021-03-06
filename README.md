# Storybook Reproduction Template for Create React App

This repro is equivalent to running:

```sh
yarn create react-app cra
cd cra
npx sb init
```

## How to create a reproduction

```sh
npx sb repro [--no-fork] react-cra repro-undefined-controls
```

This will fork the template `storybookjs/repro-react-cra` into a repro `repro-undefined-controls`, and will checkout a copy of the fork in your local directory. Passing `--no-fork` won't create a fork and will simply clone a copy down to your local machine.

From you can go into `repro-react-cra` and run:

```
yarn install
yarn storybook
```

Then you can modify the template to create a reproduction of the problem you're seeing, and commit those changes.

## How to develop against a reproduction

Inside the storybook monorepo:

```sh
yarn repro https://github.com/username/repro-undefined-controls
```

This will pull down a repro that is linked to the current development environment so that you can live-develop against the repro.
