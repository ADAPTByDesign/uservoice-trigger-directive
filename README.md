uservoice-trigger-directive
===========================
[![Build Status](https://travis-ci.org/chesleybrown/uservoice-trigger-directive.svg?branch=master)](https://travis-ci.org/chesleybrown/uservoice-trigger-directive)
[![Dependency Status](https://david-dm.org/chesleybrown/uservoice-trigger-directive.svg)](https://david-dm.org/chesleybrown/uservoice-trigger-directive)
[![devDependency Status](https://david-dm.org/chesleybrown/uservoice-trigger-directive/dev-status.svg)](https://david-dm.org/chesleybrown/uservoice-trigger-directive#info=devDependencies)
[![NPM version](https://badge.fury.io/js/uservoice-trigger-directive.svg)](http://badge.fury.io/js/uservoice-trigger-directive)

Simple directive to trigger a UserVoice widget. Requires UserVoice widget to be included.

#### Install with Bower

```
bower install uservoice-trigger-directive
```

#### Include the directive in your Angular module

```
var myApp = angular.module('myApp', ['uservoice-trigger-directive']);
```

## Usage

Use the `uservoice-trigger` directive attribute on the element you want to trigger the UserVoice widget on click. You also can change the `mode` used by setting the `mode` attribute to one of `contact`, `smartvote` or `satisfaction` (see [UserVoice docs](https://developer.uservoice.com/docs/widgets/overview/) for more information on the widget options). It is also possible to set the `position` attribute to determine which direction the widget will appear (default is `automatic`). Remember to have the `UserVoice` widget included already.

## Examples

```html
<a uservoice-trigger mode="contact">Contact</a>
<a uservoice-trigger mode="smartvote" position="top">Vote</a>
<a uservoice-trigger mode="smartvote" position="top" identify="identify">Vote</a>
```


## Running Tests

To execute all the tests, just run:

```
npm test
```
