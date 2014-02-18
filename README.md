# CASA Bootstrap

A bootstrapper that sets up an environment for the CASA reference implementation.

See [casa-environment](https://githug.com/AppSharing/casa-environment) for more details.

## Usage

### Development Environment

The environment may be downloaded and setup with the following command:

```
curl -L -0 http://appsharing.github.io/casa-bootstrap/dev | sh -s
```

This will create a `casa` directory with a number of locally linked gem repositories underneath.

The next thing that one must do is configure the gems they wish to run. This can be done by hand or with the `casa-environment` gem. To use the latter, navigate to `casa/casa-environment`. From within this directory, edit `config/dev.json` as desired and then call:

```
bundle exec thor env:dev:configure
```

See [casa-environment](https://github.com/AppSharing/casa-environment) for more details.