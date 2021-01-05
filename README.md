#### aws
> A Fish plugin for the [Amazon Web Services CLI][aws-cli]. Adapted from the [Oh My Fish!][omf] [plugin-aws][plugin-aws].

[![MIT License](https://img.shields.io/badge/license-MIT-007EC7.svg?style=flat-square)](/LICENSE)
[![Fish Shell Version](https://img.shields.io/badge/fish-v3.1.0-007EC7.svg?style=flat-square)](https://fishshell.com)


<br/>

Currently provides two integrations beyond just the base features of the [AWS CLI][aws-cli]:

- Completions, so that you don't have to memorize the hundreds of AWS subcommands
- Simple profile switching, so that you don't have to pass in `--profile` all the time

## Install

```fish
$ fisher install jerr0328/plugin-aws
```


## Usage

See the documentation for the [AWS Command Line Interface][aws-cli] on basic usage.

For profile switching, this plugin provides the `aws profile` subcommand. To switch your current profile, just provide the profile name:

```fish
$ aws profile stage
```

You can view your current profile by passing in no additional arguments:

```fish
$ aws profile
stage
```

The profiles available come from your AWS credentials file (`~/.aws/credentials`). Profile switching is very rudimentary and is just a shortcut for implicitly passing the `--profile <name>` option. If you need more robust AWS profile management, check out the [asp] plugin by [@mgoodness](https://github.com/mgoodness).

Your current profile is saved between shell sessions.


## License

[MIT][mit] © [sagebind][author] et [al][contributors]


[asp]: https://github.com/mgoodness/plugin-asp
[author]: https://github.com/sagebind
[aws-cli]: https://aws.amazon.com/cli/
[contributors]: https://github.com/jerr0328/plugin-aws/graphs/contributors
[license-badge]: https://img.shields.io/badge/license-MIT-007EC7.svg?style=flat-square
[mit]: https://opensource.org/licenses/MIT
[omf]: https://github.com/oh-my-fish/oh-my-fish
[plugin-aws]: https://github.com/oh-my-fish/plugin-aws
