# DockerPress

DockerPress makes WordPress developers life easier to develop & test WordPress
themes and plugins or even create a patch to submit to WordPress.org! This
project uses the test tools from the [wordpress-develop
repository](https://github.com/WordPress/wordpress-develop).

![](https://s.w.org/images/backgrounds/wordpress-bg-medblue.png)

## Getting Started

```sh
docker-compose up
```

**Note:** Add `--build` for the first time.

After running Docker, visit [localhost:8069](http://localhost:8069) to start
WordPress. For more information about WordPress installation, please refer to
the [Installing WordPress](https://codex.wordpress.org/Installing_WordPress/).

## Contributing to WordPress.org

See how we can create a patch
[here](https://make.wordpress.org/core/handbook/contribute/git/#patches) then
run the following commands:

```sh
$ git clone git://develop.git.wordpress.org/ wordpress-develop
$ docker-compose -f docker-compose.dev.yml up
```

**Note:** Add `--build` for the first time.

After running docker, visit [localhost:8070](http://localhost:8070).

### Running PHPUnit for WordPress

```sh
$ cp conf/wp-tests-config.php wordpress-develop
$ docker-compose exec wordpress bash
$ phpunit
```

## Contributing to This Repo

1. Fork it (<https://github.com/prontotools/docker-press/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request

<!-- Markdown link & img dfn's -->
[npm-image]: https://img.shields.io/npm/v/datadog-metrics.svg?style=flat-square
[npm-url]: https://npmjs.org/package/datadog-metrics
[npm-downloads]: https://img.shields.io/npm/dm/datadog-metrics.svg?style=flat-square
[travis-image]: https://img.shields.io/travis/dbader/node-datadog-metrics/master.svg?style=flat-square
[travis-url]: https://travis-ci.org/dbader/node-datadog-metrics
[wiki]: https://github.com/yourname/yourproject/wiki
