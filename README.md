### Simple command to generate project from this archetype
 mvn archetype:generate -DarchetypeGroupId=ru.craftcoderr.maven -DarchetypeArtifactId=liqui-base
 
### Project reconfiguration after profile change
 mvn resources:resources
 
 ### Run migrations
 mvn liquibase:update

**NOTE** Maven can be stuck on "Generating project in Interactive mode" for several seconds.

**NOTE** When you update connection profile (and firstly usage after project generated), you need to run 
 mvn resources:resources

