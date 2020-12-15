![NexT preview](https://user-images.githubusercontent.com/16272760/83972923-98baae80-a915-11ea-8142-3cf875dad8bf.png)

<a title="NexT website" href="https://theme-next.js.org"><img align="right" alt="NexT logo" width="100" height="100" src="https://raw.githubusercontent.com/next-theme/hexo-theme-next/master/source/images/logo.svg"></a>

# NexT

> «NexT» is a high quality elegant [Hexo](https://hexo.io) theme. It is crafted from scratch with love.

[![NPM version](https://img.shields.io/npm/v/hexo-theme-next?color=red&logo=npm&style=flat-square)](https://www.npmjs.com/package/hexo-theme-next)
[![Required Hexo version](https://img.shields.io/badge/hexo-%3E=5.0.0-blue?style=flat-square&logo=hexo)](https://hexo.io)
[![License](https://img.shields.io/badge/license-%20AGPL-orange?style=flat-square&logo=gnu)](https://github.com/next-theme/hexo-theme-next/blob/master/LICENSE.md)
[![Build Status](https://img.shields.io/github/workflow/status/next-theme/hexo-theme-next/Linter?label=test&logo=github&style=flat-square)](https://github.com/next-theme/hexo-theme-next/actions?query=workflow%3ALinter)
[![Build Status](https://img.shields.io/github/workflow/status/next-theme/hexo-theme-next/Tester?logo=github&style=flat-square)](https://github.com/next-theme/hexo-theme-next/actions?query=workflow%3ATester)
[![jsDelivr hits](https://img.shields.io/jsdelivr/npm/hm/hexo-theme-next?style=flat-square&logo=jsdelivr)](https://www.jsdelivr.com/package/npm/hexo-theme-next)

## Installation

If you're using Hexo 5.0 or later, the simplest way to install is through npm:

```sh
$ cd hexo-site
$ npm install hexo-theme-next
```

Or you can clone the entire repository:

```sh
$ cd hexo-site
$ git clone https://github.com/next-theme/hexo-theme-next themes/next
```

See [detailed installation instructions][docs-installation-url] if you want any other variant.

After the installation, open Hexo config file and set `theme` variable to `next`.

```yml
theme: next
```

## Configuration

At present, NexT encourages users to use the [Alternate Theme Config][docs-configuration-url] to configure NexT. And it's easy to customize the layout or style of NexT using [Custom Files][docs-custom-files-url].

It is not recommended to directly modify any files in the NexT theme. Because this may cause errors (e.g. merge conflicts), and the modified files may be discarded when upgrading the theme.

However, you can bypass merge conflicts (error message like **«Commit your changes or stash them before you can merge»**) by using the `Commit`, `Stash` or `Reset` commands for local changes. See [here](https://stackoverflow.com/a/15745424/5861495) how to do it.

## Plugins

Plugins extend and expand the functionality of NexT. There are two types of plugins: core plugins and third-party plugins. The core plugins are required by the basic functions of NexT. Third-party plugins provide a large number of optional features.

Configuring these plugins is very easy. For example, if you want to enable `pjax` on your site, just set `pjax` to `true` in NexT config file:

```yml
# Easily enable fast Ajax navigation on your website.
# For more information: https://github.com/next-theme/pjax
pjax: true
```

### Configure CDN

Third-party plugins are loaded from [jsDelivr](https://www.jsdelivr.com) CDN by default. We also provide other optional CDNs, including the famous [UNPKG](https://unpkg.com) and [CDNJS](https://cdnjs.com).

For example, if you want to use `unpkg` instead of `jsdelivr` as the default CDN provider, you need to edit the following settings in NexT config file:

```yml
vendors:
  # ...
  # Some contents...
  # ...
  plugins: unpkg
```

## Update

A new version of NexT will be released every month. You can update NexT by the following command.

Install the latest version throuth npm:

```sh
$ cd hexo-site
$ npm update hexo-theme-next
```

Or update to latest master branch:

```sh
$ cd themes/next
$ git pull
```

**If you want to update from v5.x / v7.x to the latest version, read [this][docs-update-5-1-x-url].**
