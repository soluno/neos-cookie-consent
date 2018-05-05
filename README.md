# ObisConcept.CookieConsent

A Neos CMS package that integrates [Cookie Consent](https://cookieconsent.insites.com/).

## Installation

Require it through composer:
``` shell
$ composer require obisconcept/neos-cookieconsent:^2.0.0
```

## Usage

You only need to configure the plugin through your local `Settings.yaml`.
The following options are available:

``` yaml
ObisConcept:
  CookieConsent:
    enable: true                # Wether to enable the notice
    includeJavaScript: true     # Auto-include the javascript file
    includeCss: true            # Auto-include the stylesheet
    translations:               # The translation source
      package: 'ObisConcept.CookieConsent'
      source: 'Main'
    settings:                   # CookieConsent API settings
      type: 'info'              # ('info' / 'opt-in' / 'opt-out')
      position: 'bottom'        # ('bottom' / 'bottom-left' / 'bottom-right' / 'top' / 'pushdown')
      theme: 'block'            # ('block' / 'classic' / 'edgeless' / 'wire')
      policyPage:
        node: ''                # The policy page node identifier (optional)
        section: ''             # The policy page node target anchor (optional)
      palette:                  # The color palette of the notice
        popup:
          background: '#000'
          text: '#fff'
        button:
          background: '#f1d600'
          text: '#000'
```
