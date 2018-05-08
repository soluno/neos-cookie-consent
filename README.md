# ObisConcept.CookieConsent

A Neos CMS package that integrates [Cookie Consent](https://cookieconsent.insites.com/).

**Please notice** that this branch has been created to serve legacy Neos versions between 2.0 and 2.3! It is not a stable branch and should not be used in production systems!

## Installation

Require it through composer:
``` shell
$ composer require obisconcept/neos-cookieconsent:dev-2.0-legacy
```

## Usage

You only need to configure the plugin through your local `Settings.yaml`.
The following options are available:

``` yaml
ObisConcept:
  CookieConsent:
    enable: true                # Wether to enable the notice.
    includeJavaScript: true     # Auto-include cookieconsent's javascript file.
    includeCss: true            # Auto-include cookieconsent's stylesheet file.
    policyPageNode: ''          # The page identifier of your privacy statement.
    translations:               # Change the translation source for custom texts.
      package: 'obisconcept.neoscookieconsent'
      source: 'Main'
    position: 'bottom'          # The position of the notice. Possible Values:
                                # "bottom", "bottom-left", "bottom-right", "top"
    theme: 'block'              # The theme of the notice. Possible Values:
                                # "block", "classic", "edgeless", "wire"
    palette:
      popup:
        background: '#000'      # The background color and
        text: '#fff'            # the text color of the notice box
      button:
        background: '#f1d600'   # The background color and
        text: '#000'            # the text color of the dismiss-button
```
