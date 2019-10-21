# Housekeeping

The purpose of this repository is to hold all necessary housekeeping information for the development of the ocibuilder project.

## Standups

Standups will occur on **Monday, Wednesday** and **Friday** at **9:15/12:15/17:15** PST/EST/GMT on a weekly basis.

Standups will last 15 minutes and will answer the following:
* What was done yesterday?
* What is being worked on today?
* Any blockers?
* Any other escalated problems


## Sprint Planning

Sprint planning will take place on **Monday** at the start of each sprint.

Each issue in the backlog will be given a priority, assigned to a developer and assigned a milestone if appropriate.

## Issues

Issues relating to ocibuilder are stored [here](https://github.com/ocibuilder/ocibuilder/issues)

* All issues relating to ocibuilder will be tracked on the single board
* Issues must follow the *feature* and *bug* templates that have been defined
* Issues must be categorised into **enhancement**, **feature**, **bugfix**, **documentation** or **testing** through labels
* Issues can be prioritised as follows:
    * **PRIORITY: 1** - to be picked up and resolved in the current sprint
    * **PRIORITY: 2** - to be groomed, requirements to be defined and to be ready to be picked up in the upcoming sprint
    * **PRIORITY: 3** - in the backlog, waiting to be groomed
    * **PRIORITY: 4** - nice to have
* If an issue has been picked up for the current sprint, a milestone should be assigned
* Issues can be linked to the [project board](https://github.com/ocibuilder/ocibuilder/projects/1) and it's status should be tracked and updated 

## Releases

Releases will be published to GitHub [here](https://github.com/ocibuilder/ocibuilder/releases)

* Releases require updating [VERSION](https://github.com/ocibuilder/ocibuilder/blob/master/VERSION) to match the latest milestone
* The ocibuilder follows [semantic versioning](https://semver.org/)
* A release is triggered by dropping a tag of the version onto the repository. This will trigger the pipeline to release the artifacts.
* The artifacts that will be released are as follows:
    * Linux binary of `ocictl`
    * Mac binary of `ocictl`
    * A docker image of `ocictl` with *buildah* and *docker* dependencies
* Release binaries will be stored in github releases
* Release images will be pushed to the [ocibuilder dockerhub registry](https://cloud.docker.com/u/ocibuilder/repository/docker/ocibuilder/ocictl)

## Milestones

Milestones are tracked on Github and available [here](https://github.com/ocibuilder/ocibuilder/milestones)

* A milestone represents a release at the end of each **2** week sprint
* A milestone is named with the following structure `release <RELEASE_VERSION>` e.g. `release v0.1.0`
* Each milestone should contain a description which outlines which is to be released at the due date
* Each milestone will have a due date which will be set as the date of the end of the sprint

## Pull Requests

The following are guidelines for pull requests in the ocibuilder project.

* All code is to be approved by a listed maintainer before it can be merged into master
* Code must also pass any necessary checks as part of the build pipeline found [here](https://circleci.com/gh/ocibuilder)
* Any pull requests will be checked for code coverage - with no approvals being granted if the overall code coverage of the project has decreased
* All new features or enhancements must be unit tested
* Pull requests raised by the active maintainers must be addressed within **2** days or will be escalated
* Pull requests raised by external contributors will be addressed within **4** days or will be escalated
* Standard go review guidelines and comments are defined in the [common golang comments](https://github.com/golang/go/wiki/CodeReviewComments) and in [effective go](https://golang.org/doc/effective_go.html)

## Active Maintainers

* [Art Begolli](https://github.com/artbegolli)
* [Vaibhav Page](https://github.com/VaibhavPage)
* [Aniket Kulkarni](https://github.com/AniketKul)


* [Mike Bowen](https://github.com/orgs/ocibuilder/people/michael-bowen-sc)