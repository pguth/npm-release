# npm-release

A little script to help release `npm` modules. It:

- Bumps the version in `package.json`
- Commits 'Release v<version number>'
- Tags
- Pushes the commit & tag (`git push && git push --tags`)
- Releases to npm (with `npm publish`)

## Usage

You must use `npm-release` in a folder with a `package.json` and a remote to push to.

`npm-release 0.0.2`

It supports the same version options as `npm version`.

`npm-release [<newversion> | major | minor | patch | build]`

And custom commit messages:

`npm-release major -m "#yolo"`

Finger-licking good!

## Install

`npm install -g npm-release`

## License

MIT