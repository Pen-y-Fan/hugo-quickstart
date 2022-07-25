# Quickstart for Hugo

Quickstart for [Hugo](https://gohugo.io/getting-started/quick-start/) static site generator, to get the first project up and running

## Installation

Required

- [Go](https://go.dev/) download and install or use a docker container
- [Hugo](https://gohugo.io/getting-started/) download and add to your PATH to allow it to be executable

Recommended:

- [Git](https://git-scm.com/downloads)

### Clone

See [Cloning a repository](https://help.github.com/en/articles/cloning-a-repository) for details on how to create a
local copy of this project on your computer.

e.g.

```sh
clone git@github.com:Pen-y-Fan/hugo-quickstart.git
cd hugo-quickstart
```

### Add theme

The theme has been included as a git submodule, it needs to be initialised too.

```shell
git submodule update --init
```

## Commands

Basic commands

### Create a post

To create a new post **My second post** in the **posts** directory. Note the kebab case (url friendly) for the markdown
file name.

```shell
hugo new posts/my-second-post.md
```

### Server

Use the hugo server to check the current state of the development site (-D includes draft pages)

```shell
hugo server -D
```

The website can be accessed from <localhost:1313>

### Deploy

Once the new content has been checked, you are ready to deploy

1. check `draft: false` is set in the front matter
2. deploy the latest additions to the **public** directory:

```shell
hugo -D
```

## License

MIT License (MIT). Please see [License File](LICENSE.md) for more information.
