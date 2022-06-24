# AZ Grad College Webform Elements
## For Quickstart 2 / Drupal 9+

Provides webform elements, especially select options, from dynamic JSON sources.

## Installation

Assuming you have a Quickstart 2 site's git repository cloned, edit your site's 
`composer.json` file.

Add the following to the `repositories` section:

```json
  {
    "type": "vcs",
    "url": "git@github.com:uazgraduatecollege/azgrad_drupal_webform_elements.git"
  }
  ```
And add the following to the `require` section:

```json 
  {
    "uazgraduatecollege/azgrad_drupal_webform_elements": "dev-main"
  }
```

Commit your changes and re-initialize you site.

If using a site cloned from Pantheon, delete your `composer.lock` file before
committing your changes and then `git push` back up to the pantheon remote.

## Configuration 

Enable the by navigating to your site's `Admininistration => Extend` and clicking 
the AZ Grad Webform Element module.

Alternatively, enable using terminus:

```sh
$ terminus remote:drush en azgrad_drupal_webform_elements 
```

The elements provided by this module should now be ready to use in Drupal webforms.

## Notes

