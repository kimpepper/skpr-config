# Skpr Config

A simple utility for reading skpr config from a directory, and populating
environment variables.

The default skpr config directory is /etc/skpr

## Usage

```
$config = SkprConfig::create()->load();
$config->get('foo.bar')
```

Skipper config variables will be converted to uppercase, and dots are
converted to underscores. For example:

```
getenv('FOO_BAR')
```

## Testing

Run tests using the following:

`bin/phpunit`

## Code Standards

Run code style checks with the following:

`bin/phpcs`
