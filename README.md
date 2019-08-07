# WYSIWYG + VisualCMS replacement if modules are not used

This package removes the unused OXID WYSIWYG + VisualCMS module packages from the shop and prevents conflicts in later updates.

## Install

if the WYSIWYG + VisualCMS modules are not used and should be removed from the shop installation

* Deactivate the WYSIWYG + VisualCMS modules in the shop backend.
* Run this composer statement in your shop. Adjust this instruction if your installation requires it.

    `composer require d3/oxid-wysiwyg-replacement --update-no-dev`
    
* Manually remove the files from source/modules/ddoe/visualcms and source/modules/ddoe/wysiwyg.

## Uninstall

if the WYSIWYG + VisualCMS modules are to be used again

* Manually clean up the replacement module entry (d3/oxid-wysiwyg-replacement) from the vendor/composer/installed.json and composer.lock files.
* Run this composer statement in your shop. Adjust this instruction if your installation requires it.

    `composer remove d3/oxid-wysiwyg-replacement --update-no-dev`
