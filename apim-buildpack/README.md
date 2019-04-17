# WSO2 API Manager Cloud Foundry Buildpack

The `apim-buildpack` is a [Cloud Foundry][] buildpack for running WSO2 API Manager based applications.  It is designed to run many WSO2 API Manager based applications (TODO: examples here) with no additional configuration, but supports configuration of the standard components.

## Usage
To use this buildpack specify the URI of the repository when pushing an application to Cloud Foundry:

```bash
$ cf push <APP-NAME> -p <ARTIFACT> -b https://github.com/wso2/apim-buildpack.git
```

## Examples
The following is _very_ simple example for deploying the artifact types that we support.

* [Pizzashack project](samples/micro-gw-pizzashack-project/micro-gw-pizzashack-project.md)

## Building Packages
The buildpack can be packaged up so that it can be uploaded to Cloud Foundry using the `cf create-buildpack` and `cf update-buildpack` commands.  In order to create these packages, the rake `package` task is used.

Note that this process is not currently supported on Windows. It is possible it will work, but it is not tested, and no additional functionality has been added to make it work.


## License
This buildpack is released under version 2.0 of the [Apache License][].

[Apache License]: http://www.apache.org/licenses/LICENSE-2.0
[Cloud Foundry]: http://www.cloudfoundry.org
[Environment Variables]: http://docs.cloudfoundry.org/devguide/deploy-apps/manifest.html#env-block
[GitHub's forking functionality]: https://help.github.com/articles/fork-a-repo
[pull request]: https://help.github.com/articles/using-pull-requests
[Pull requests]: http://help.github.com/send-pull-requests
[Wikipedia]: https://en.wikipedia.org/wiki/YAML#Basic_components_of_YAML
