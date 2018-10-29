WP-CLI Bundle
======

Bundle WP-CLI into a phar. 

--------------------------------------------------------------

### This version was forked to keep it compatible with Windows for things like `wp shell`

Forked with the following customizations:
1. Support `wp shell` on windows.
2. Pass a custom output directory for the bundled `wp-cli.phar` file.

--------------------------------------------------------------------------------------------------------------------------------------

### Building a `wp-cli.phar`
1. Clone or download this repo.
2. Run `composer install` from the root directory.
3. Run the following command while specifying an output directory.

```bash
bash ./utils/update-phar <output directory>
```

