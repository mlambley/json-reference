# JSON Reference

# Maintained Once Again!

This project was originally forked from thephpleague who is no longer maintaining it.
However this library is the best json dereferencer I can find, so I will continue to maintain it.

Please log any issues or feature requests [here](https://github.com/mlambley/json-reference/issues)

-----

Most JSON schemas use JSON references to minimize duplication. A JSON reference is an object that looks like {"$ref": "http://some/where"} and points to a JSON object somewhere else.

JSON Reference is a library for resolving references.

- Resolves all references, replacing them with proxy objects.
- Supports references to external files, urls, or custom sources.
- Safely resolves circular references.
- Supports caching dereferenced schemas.
- Dereferenced schemas can be safely json_encoded.
- Works with Swagger, JSON Schema, and any other spec compliant JSON documents.

## Install

### Via Composer

```bash
composer require mlambley/json-reference
```

## Usage

Complete documentation is available [here](http://json-reference.thephpleague.com/)

## Change log

Please see [CHANGELOG](CHANGELOG.md) for more information about what has changed recently.

## Testing

``` bash
$ composer test-server
$ composer test
```

## Benchmarks

The benchmarks require a local redis server to be running on localhost at the default port.

```bash
$ composer bench
```

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Credits

- [Matt Allan][link-author]
- [All Contributors][link-contributors]

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.