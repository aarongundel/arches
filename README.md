# Arches

Arches is a web-based, geospatial information system for cultural heritage inventory and management. Arches is purpose-built for the international cultural heritage field, and designed to record all types of immovable heritage, including archaeological sites, buildings and other historic structures, landscapes, and heritage ensembles or districts. For more information and background on the Arches project, please visit [archesproject.org](http://archesproject.org/).

For general inquiries and to get technical support from the wider Arches community, visit our [Community Forum](https://community.archesproject.org/).

For general user installation and app documentation, visit [arches.readthedocs.io](https://arches.readthedocs.io).

For the documentation pertaining to the bleeding edge code (what is in the ``master`` branch), visit [arches.readthedocs.io/en/latest](https://arches.readthedocs.io/en/latest).  We welcome new contributors; please see [Contributing to Arches](CONTRIBUTING.md) for details.

Issue reports are encouraged! [Please read this article](http://polite.technology/reportabug.html) before reporting issues.
*   [Report a Bug](https://github.com/archesproject/arches/issues/new?template=bug.md)
*   [File a Feature Ticket](https://github.com/archesproject/arches/issues/new?template=feature.md)

[Version 7.4.2 release notes](https://github.com/archesproject/arches/blob/dev/7.4.x/releases/7.4.2.md)

#### Quick Install

Installation is fully documented in the official documentation, [arches.readthedocs.io/en/stable](https://arches.readthedocs.io/en/stable), but assuming you have all of the dependencies installed you should make a virtual environment, activate it, and then run
```
    pip install arches
```
then
```
    arches-project create myproject
```
enter the new `myproject` directory
```
    cd myproject
```
and run
```
    python manage.py setup_db
    python manage.py runserver
```
in a separate terminal, activate your virtual environment and navigate to the root directory of the project ( you should be on the same level as `package.json`) 
```
    cd myproject/myproject
```
and run
```   
    yarn build_development
```
to create a frontend asset bundle. This process should complete in less than 2 minutes.

Finally, visit `localhost:8000` in a browser (only Chrome is fully supported at this time).

If you run into problems, please review our full [installation documentation](http://arches.readthedocs.io/en/stable/installation/)

#### Release Cycle

Our general release cycle will typically be a functional release (either major if there are backward incompatible changes or minor, if there are not) every 6 months. Each functional release will typically be followed by one or more patch releases. See [semver.org](https://semver.org/) for version numbering.

-   Functional releases will usually introduce new functionality to the application, but could also include styling updates, enhancements to the UX, bug fixes, and performance improvements.
-   Patch releases are really only concerned with fixing any bugs related to the previous release or any other issues not yet addressed

#### Support for previous releases

- Stable releases will be supported with patch releases for at least 18 months. Typically the stable release will be the second or third minor release of a major release. 
- Functional releases (with the exception of stable releases) will be supported only until the next functional release. After that users are expected to upgrade to the latest release on [pypi.python.org](https://pypi.python.org/pypi/arches)

#### Feature roadmap

The following a general plan for the Arches project. Be aware this plan is tentative and subject to change

## 7.5 - Release date: December 15, 2023 
- Continued accessibility improvements
- Arches application support
- Bulk Data Manager export
- Bulk Data Manager deletion
- Tile Excel format added to Bulk Data Manager
- Improved Bulk Data Manager data edting
- Workflow history tracking
- Image configuration of file-list datatype
- Perfomance Improvements
- Support for component authoring in Vue Javascript framework

## 7.6 - Release date: June 15, 2024
- Activity stream edit logs
- User specific saved searches
- Security enhancements

## 8.0 - Release date: December 15, 2024
- Migrate Arches UI Framework
- Support for editing and publishing graphs (removing instance restrictions)
- Support for viewing and restoring previous graph publications
- Support for editing/localizing UI labels and permissions for published graphs
- Business data migrations that correspond to graph changes
- RDM Redesign

