# Create React App

This repro is equivalent to running:

```sh
yarn create react-app cra
cd cra
npx sb init
```

## How to create a reproduction

```sh
npx sb repro react-cra repro-undefined-controls
```

This will fork the template `storybookjs/repro-react-cra` into a repro `repro-undefined-controls`, and will checkout a copy of the fork in your local directory.

To clone this to your local machine without creating a fork:

```sh
npx sb repro --no-fork react-cra repro-undefined-controls
```

## How to develop against a reproduction

Inside the storybook monorepo:

```sh
yarn repro https://github.com/username/repro-undefined/controls
```

This will pull down a repro that is linked to the current development environment so that you can develop against the repro.
