# JSON Testing

This project tests various interlok-json related components and
features.

## interlok-json-web-token

The JSON web token workflow contains two services, one for creating a
JWT and a second for decoding that result. The service tester tests the
decode service and verifies that the claims and metadata are as
expected.

## interlok-jq

The JSON JQ service and test verify the workings of the
json-jq-transform service, and that unformatted JSON is properly
formatted as expected.

## interlok-json

### Path

Test that the JSON path service can correctly extract a JSON object from
a larger JSON object, using a JSON path expression.

### XML Transforms

There are two tests: JSON -> XML and XML -> JSON.

### JSON Transform

Tests the JSON transform service, which allows JSON -> JSON
transformations to be made. The service takes source JSON content and
applies the transform definition, the result of which will be more JSON
content.

### Getting started

* `./gradlew clean build`
* `(cd ./build/distribution && java -jar lib/interlok-boot.jar)`