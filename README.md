WP-CLI Bundle
======
Bundle WP-CLI into a phar.

<p>
<a href="https://github.com/lipemat/wp-cli-bundle/releases/latest">
<img alt="Package Version" src="https://img.shields.io/github/v/tag/lipemat/wp-cli-bundle?label=version"/>
</a>
</p>


### This version was forked to keep it compatible with Windows for things like `wp shell`

Forked with the following customizations:

1. Support `wp shell` on Windows.
2. Pass a custom output directory for the bundled `wp-cli.phar` file.
3. Pass a custom version to the bundled `wp-cli.phar` file.
4. Support `wp rest` commands from [wp-restful](https://github.com/lipemat/restful).

--------------------------------------------------------------------------------------------------------------------------------------

### Downloading `wp-cli.phar`

You may download
that <a href="https://github.com/lipemat/wp-cli-bundle/releases/latest/download/wp-cli.phar">
latest wp-cli.phar here</a> or previous versions from
the <a href="https://github.com/lipemat/wp-cli-bundle/releases/">Releases section</a>.

### Building a `wp-cli.phar`

1. Clone or download this repo.
2. Run `composer install` from the root directory.
3. Run the following command while specifying an output directory.

```bash
bash ./utils/update-phar <output directory> <version>
```

Example

```
bash ./utils/update-phar E:/scripts/wordpress 2.5.0-windows
```

-------------------------------------------------------------------

### Running from source

1. Run `composer install` from the root directory.
2. Run the executables found in `vendor/wp-cli/wp-cli/bin` from the WordPress site root.
   E.G. `E:/SVN/wp-cli-bundle/vendor/wp-cli/wp-cli/bin/wp option get siteurl`

-----------------------------------------------------------------------------------


wp-cli/wp-cli-bundle
=================


Combines the most common commands into the standard, installable version of WP-CLI.

Generally, bundled commands either relate directly to a WordPress API or offer some common developer convenience. New commands are included in the WP-CLI bundle when the [project governance](https://make.wordpress.org/cli/handbook/contributions/governance/) decides they should be. There isn't much of a formal process to it, so feel free to ask if you ever have a question.

The handbook documents the [various ways you can install the bundle](https://make.wordpress.org/cli/handbook/guides/installing/). The Phar is [built on every merge](https://github.com/wp-cli/wp-cli-bundle/blob/main/.github/workflows/deployment.yml) and pushed to [wp-cli/builds](https://github.com/wp-cli/builds) repository. A stable version is [tagged a few times each year](https://make.wordpress.org/cli/handbook/contributions/release-checklist/).
Both `wp-cli/wp-cli` and `wp-cli/wp-cli-bundle` use milestones to indicate the next stable release. For `wp-cli/wp-cli`, the milestone represents the version of the WP-CLI framework. For `wp-cli/wp-cli-bundle`, the milestone represents the WP-CLI Phar version. We keep these in sync for backwards compatibility reasons, and to avoid causing confusion with third party commands. Each of the command repositories are versioned independently according to semantic versioning principles as needed.
