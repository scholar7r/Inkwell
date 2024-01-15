# Inkwell

A retro, clean and elegant Hugo blog theme.

## Installation

To install Inkwell, you can use either of the following two methods. The most standard method is to use the Submodule method, which can smoothly transition to each new version. If you have some understanding of Hugo's theme programming and need to customize the theme, then the installation method of the Clone code repository is more recommended.

Before the following steps, please ensure that you have completed initialization through Hugo CLI. If you need to use the submodule method for installation, please perform Git initialization.

### Submodule installation

```Shell
# Add submodule
Git submodule add https://github.com/scholar7r/Inkwell.git themes/inkwell
# Update submodule
Git submodule update --init --recursive
# Remote update
Git submodule update --remote
```

At this point, the Submodule has been created in the `themes/inkwell` directory. Next, copy the necessary files from the `exampleSite` directory to the Hugo directory.

### Clone code repository

```Shell
# Clone code repository
Git clone https://github.com/scholar7r/Inkwell.git themes/inkwell
```

At this point, the Inkwell repository has been cloned, and you can modify certain template files according to your needs.

### Copy necessary files

After the theme installation is completed, some files from `exampleSite` need to be copied to the Hugo root directory.

```
exampleSite
├── assets
├── content
├── i18n
└── hugo.toml
```

The exampleSite directory contains customizable folders for `assets`, `content`, and `i18n`, as well as the `hugo.toml` configuration file template.

In general, you only need to copy these three folders and one configuration file to the Hugo root directory.

```Shell
# Copy necessary files
cp themes/inkwell/exampleSite/* .
```
