# OWASP CRS - ActivityPub Rule Exclusions Plugin
![Integration tests](https://github.com/coreruleset/template-plugin/actions/workflows/integration.yml/badge.svg)

An OWASP CRS Rule exclusions plugin for legitimate ActivityPub requests. This is an experimental plugin and is mirrored from [git.open.engineering](https://git.open.engineering/oeng/activitypub-rule-exclusions-plugin) to the following locations:

- [Codeberg](https://codeberg.org/open-engineering/activitypub-rule-exclusions-plugin) (please submit Issues and PRs here)
- [GitHub](https://github.com/jessebot/activitypub-rule-exclusions-plugin)

The CRS plugin documentation can be found on the [website](https://coreruleset.org/docs/configuring/plugins/).

## Testing

Plugins can also be shipped with their own tests. Any `ftw` test yaml file that you add below the `tests/regression` directory will be run by the integrated pipeline.
We suggest you to use a new subdirectory for your specific plugin's test, e.g. `tests/regression/<your-plugin>`, and create one file per rule you want to test.

Many plugins target rule exclusions, so it will be rather common to see tests matching a REQUEST_URI but matching for `no_log_contains`, as we want to test that we are not being blocked.

## License

Copyright (c) 2021-2022 OWASP CRS project. All rights reserved.

The OWASP CRS and its official plugins are
distributed under Apache Software License (ASL) version 2.
Please see the enclosed LICENSE file for full details.
