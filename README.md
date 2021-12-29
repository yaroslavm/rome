# Rome

[![Build](https://github.com/rometools/rome/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/rometools/rome/actions/workflows/build.yml)
[![Maven Central](https://maven-badges.herokuapp.com/maven-central/com.rometools/rome/badge.svg)](https://maven-badges.herokuapp.com/maven-central/com.rometools/rome)

Rome (**R**SS and AT**OM** utiliti**e**s) is a Java framework for RSS and Atom feeds.

## Project structure

| Module         | Description                                                            | Links                         |
| -------------- | -----------------------------------------------------------------------| ------------------------------|
| `rome`         | Maven parent project (dependency Management, build configuration, etc) |                               |
| `rome-core`    | Core library for generating, parsing and converting RSS and Atom feeds | [Documentation](rome-core)    |
| `rome-modules` | Support for extensions like MediaRSS, GeoRSS and others                | [Documentation](rome-modules) |
| `rome-opml`    | Support for [OPML](https://en.wikipedia.org/wiki/OPML)                 | [Documentation](rome-opml)    |
| `rome-utils`   | Internal utility classes                                               |                               |

## Building from source

This project can be build and published to your local Maven cache using the [Maven Wrapper](https://maven.apache.org/wrapper/). You also need JDK 11.

```sh
./mvnw clean install
```

## Development

This project uses [Lombok](https://projectlombok.org/) to reduce boilerplate code. For installation instructions please have a look at the website.

TODO
