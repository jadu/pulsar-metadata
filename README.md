# Metadata

Provides a simple way to mark up key/value information provided by a Twig hash
or JSON object.

## Example usage

```twig
{{
    html.metadata({
        'items': {
            'File': 'true_lies.avi',
            'Size': '1.2 Gb',
            'Type': 'Video'
        }
    })
}}
```

## Options

Option | Type   | Description
------ | ------ | --------------------------------------------------------------
class  | string | CSS classes, space separated
id     | string | A unique identifier, if required
items  | hash   | A hash of data where key: value = title: description
data-* | string | Data attributes, eg: `'data-foo': 'bar'`