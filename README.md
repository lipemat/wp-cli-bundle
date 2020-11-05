WP-CLI Bundle
======
Bundle WP-CLI into a phar.

<p>
<a href="https://github.com/lipemat/wp-cli-bundle/releases/latest">
<img src="https://img.shields.io/github/v/tag/lipemat/wp-cli-bundle?label=version"/>
</a>
</p>

--------------------------------------------------------------

### This version was forked to keep it compatible with Windows for things like `wp shell`

Forked with the following customizations:
1. Support `wp shell` on windows.
2. Pass a custom output directory for the bundled `wp-cli.phar` file.
3. Pass a custom version to the bundled `wp-cli.phar` file.
3. Support `wp rest` commands from [wp-restful](https://github.com/lipemat/restful).

--------------------------------------------------------------------------------------------------------------------------------------
### Downloading `wp-cli.phar`
You may download that <a href="https://github.com/lipemat/wp-cli-bundle/releases/latest/download/wp-cli.phar">latest wp-cli.phar here</a> or previous versions from the <a href="https://github.com/lipemat/wp-cli-bundle/releases/">Releases section</a>.

### Building a `wp-cli.phar`
1. Clone or download this repo.
2. Run `composer install` from the root directory.
3. Run the following command while specifying an output directory.

```bash
bash ./utils/update-phar <output directory> <version>
```
Example
```
bash ./utils/update-phar E:/scripts/wordpress 2.4.1-windows
```

-------------------------------------------------------------------
### Running from source
1. Run `composer install` from the root directory.
2. Run the executables found in `vendor/wp-cli/wp-cli/bin` from the WordPress site root. E.G. `E:/SVN/wp-cli-bundle/vendor/wp-cli/wp-cli/bin/wp option get siteurl`
