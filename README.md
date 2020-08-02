### Simple command to generate project from this archetype
 mvn archetype:generate -DarchetypeGroupId=ru.craftcoderr.maven -DarchetypeArtifactId=liqui-base
 
### Project reconfiguration after profile change
 ```mvn resources:resources```
 
### Run migrations
```mvn liquibase:update```

### Notes

* Maven can stuck on "Generating project in Interactive mode" for several seconds.
* When you updating connection profile (or firstly using after project generated), you need to run ```mvn resources:resources```

