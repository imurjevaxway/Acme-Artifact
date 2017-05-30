# Acme-Artifact
Sample artifact illustrating the guidelines for product's GitHub organizations
## Description
_definition of the repository and artifact. Concise definition of the problem it solves or value it brings. Reference to target user / environment._

## Product version dependency
_list the required product versions for this or other axway and 3rd party products which are prerequisite for using this artifact_
This artefact was successfully tested for the following versions:
- v1.2.3


## Usage
_describe how to install, deploy and start using the artifact. Provide any gotchas related to usage, deployment or initial configuration._

### Deploy
Deploy like this:
* copy files into './extentions/acmesample' directory in your product root folder
* restart your prouct or hit bounce button by going to menu->configuration in the GUI

### Uninstall
you can uninstall completely or temporarily disable this extention:
* Disable - just call 'touch ./extentions/acmesample/.bypass' and restart/bounce in your product
* Unistall:
..* Stop your product
..* remove './extentions/acmesample'
..* Restart

### Change logging storage location and rollover
By default acme sample logs to './extentions/acmesample/logs', the logs are rolled over daily. If you wish to change the location or rollover you need to do the following:
* Open './extentions/acmesample/acmesample.conf' and change the value for '[Loginto]', give your new log file location (path is relative to './extentions/acmesample' and cannot be above outside this directory
* locate '[logrolloverinterval]' and change the value in minutes; this will make logs to rollover after this many minutes has passed.


## Bug and Caveats


## Contributing

TBD

## Team

![alt text][Axwaylogo] Axway Team

[Axwaylogo]: https://github.com/Axway-API-Management/Common/blob/master/img/AxwayLogoSmall.png  "Axway logo"


## License
Apache License 2.0 (refer to document [license] (/LICENSE))

