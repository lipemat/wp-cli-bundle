WP-CLI Bundle - Windows Fork
======
A maintained fork of [WP-CLI](https://github.com/wp-cli/wp-cli-bundle) to build a `wp-cli.phar` for Windows.

<p>
	<a href="https://github.com/lipemat/wp-cli-bundle/releases/latest">
		<img alt="Package Version" src="https://img.shields.io/github/v/tag/lipemat/wp-cli-bundle?label=version"/>
	</a>
 	<img alt="WordPress" src="https://img.shields.io/badge/wordpress->=5.8.0-green.svg">
  	<img alt="PHP" src="https://img.shields.io/badge/php->=7.4.0-brown.svg" />
</p>


## Forked with the following customizations:

1. Support `wp shell` on Windows.
2. Pass a custom output directory for the bundled `wp-cli.phar` file.
3. Pass a custom version to the bundled `wp-cli.phar` file.
4. Support `wp rest` commands from [wp-restful](https://github.com/wp-cli/restful).
5. Support `wp profile` commands from [wp-profile](https://github.com/wp-cli/profile-command).

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
