# Liqui-Base

## Description

This maven archetype provides basic setup for liquibase-maven-plugin.

## Usage

### Installation and initialization
1. Clone this repo
1. Install maven archetype (run `mvn install` in root of cloned repo)
1. Cd to path where you want create maven project
1. Run `mvn archetype:generate -DarchetypeGroupId=ru.craftcoderr.maven -DarchetypeArtifactId=liqui-base` to generate project from archetype, artifactId would be used for folder name of maven project
1. Setup JDBC connector dependency in `pom.xml`
1. Setup "test" profile file `src/main/profiles/test.properties` with

        profile...
        profile.username=
        profile.password=


1. Run `mvn resources:resources` for project initialization

### Reconfiguration after profile changed
Run `mvn resources:resources`

### Running migrations
Run `mvn liquibase:update`

## Notes

* Maven can stuck on "Generating project in Interactive mode" for several seconds.


