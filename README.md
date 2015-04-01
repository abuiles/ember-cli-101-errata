ember-cli-101-errata
====================

Errata of the Ember.js book https://leanpub.com/ember-cli-101.

#### Add "Plugins.min.css" to Brocfile.js
On page 49 (book version downloaded from 3/30/15 email update), the following line needs to be added to the Brocfile.js instructions for Picnic css dependency:

    app.import('bower_components/picnic/releases/plugins.min.css');

This is needed for the "-header.hbs" `<nav>` UI element (introduced on page 51) to get its Picnic styling which is not included in the plain picnic.css but is included in Picnic's plugins.css
[Related to Issue: Page 49: Need to add Picnic's "plugins.min.css" to Brocfile.js #193] (https://github.com/abuiles/ember-cli-101-errata/issues/193)
