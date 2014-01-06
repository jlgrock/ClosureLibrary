ClosureLibrary
==============

A Simple Project that downloads the current Closure Library and will publish it as a maven artifact.

This also is a great way for others to learn how to publish JavaScript libraries as artifacts in 
Maven.  That way, people using Maven as their primary build tool can take it and use it in their
projects with ease and use all of the Maven tools that are already created.


## Requirements
Requires you to install the following:

* C-shell
* Git or Subversion
* Ant
* Maven

## Instructions on Use

1. Clone this repo
2. run `ant createPomFromInput -Drepo.version=x` (replacing 'x' with the version) or, if you just want the most recent version, run `ant createPomFromGit`
3. Commit your changes locally (which should only be the generated pom file)
4. Run the release with the profile to perform releases with `mvn release:clean release:prepare release:perform`

