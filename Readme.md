jquery-chosen-sortable fork by [@antom](http://github.com/antom)
================================================================

## Version: 1.0.1 ##

### About ###

This JQuery plugin adds JQuery UI sortable functionality to multiple selects and allows the order of selection to be maintained. The original was coded by Yves Van Broekhoven & Simon Menke on 2012-07-05 and forked by [Andy Thomas](http://github.com/antom) on 2014-08-04.

The fork adds the following features not found in the original:

- Updated to use the 'chosen-' class prefix used by newer versions of Chosen, but with backward compatibility for versions still using the old 'chzn-' one.
- Checks that JQuery UI is loaded.
- Sizes the placeholder equal to the option being dragged.

### Usage ###

Simply add the additional `chosen-sortable` class to any `<select multiple>` tag on your page and make sure that you include both JQuery UI and this plugin, eg:

```
  <script src="//ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
  <script src="//ajax.googleapis.com/ajax/libs/jqueryui/1.11.0/jquery-ui.min.js"></script>
  <script src="//path/to/jquery-chosen-sortable.min.js"></script>
```

The placeholder style should have the same margin as the `.chosen-container-multi .chosen-choices li.search-choice` to make things a little tidier, eg:

```
.chosen-container-multi .chosen-choices li.search-choice-placeholder {
  border: 1px dashed #aaa;
  margin: 3px 0 3px 5px;
}
```