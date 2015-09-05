# dls

Whenever I look into a package to learn about the packags it depended on,
I have to run `npm view` several times to get what they are.
It's boring, so I write this little tool. It can make a list of
the dependencies of a package and output it as a markdown file,
then I can view all the information in a markdown previewer.

`dls` means "dependencies ls",
it lists the dependecies/devDependecies/OptionalDependecies.
However it doesn't recursively list all the dependecies.

## Usage

```shell
npm i -g dls
# list the dependencies through the package.json in the current working directory
dls
# list the dependencies of a specified package
dls express
```

Notice: `dls` can only get the package.json of a package from the npm registry.
it will fail if the package doesn't exist in the npm registry.

## License

MIT (c) Ivan Yan
