# resolve-to-empty

This is an empty package to be used in yarn resolutions. As yarn does not support ignoring some packages installations, this is a hack to do such things by resolving the package you don't want to install to this empty package.

Issue in yarn:

https://github.com/yarnpkg/yarn/issues/4611

At the time of this writing, this package was necessary to do this easily. This might have changed when you're reading this. So please refer to the issue updates in-case of a better way to do it.

## Install

```sh
yarn add resolve-to-empty
```

## Usage

https://yarnpkg.com/lang/en/docs/selective-version-resolutions/

## Example

```json
{
  "resolutions": {
    "annoying-dependency-you-dont-want": "https://registry.npmjs.org/resolve-to-empty/-/resolve-to-empty-1.0.0.tgz"
  }
}
```
