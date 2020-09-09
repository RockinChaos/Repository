<p align="center">
 See <a href="https://github.com/RockinChaos/Repository/wiki">Repository Wiki</a> for the full detailed documentation on the usage.<br>
</p>

## Repository - [maven-public]
This repository is comprised of compiled snapshots and releases of CraftationGaming's Java resources in the form of a Maven Repository.

-----
### How to use this Repository
You can use this Repository with both Maven and Gradle.
----

####Import with Maven
----
* You can copy-paste the information below into your maven pom.xml
* Simply replace the groupId with the project path found in this Repository, an example would be `me.RockinChaos.itemjoin`
* The artifactId is the name of the project, such as `ItemJoin`
* The version can be either a SNAPSHOT or RELEASE, an example is `5.0.7-RELEASE`
  * The current versions can be found by browsing the project path in this Repository.
```
    <!--CraftationGaming Repository-->
        <repository>
            <id>CraftationGaming</id>
            <url>https://raw.githubusercontent.com/RockinChaos/repository/maven-public/</url>
        </repository>

    <!--Project API-->
        <dependency>
            <groupId>project.path</groupId>
            <artifactId>projectName</artifactId>
            <version>project-version</version>
            <scope>provided</scope>
        </dependency>
```
----

####Import with Gradle
----
* You can copy-paste the information below into your Gradle configuration, nothing should need to be changed.
```
plugins {
    id "com.github.unafraid.gradle.git-repo-plugin" version "2.0.4.1"
    id "java"
    id "maven-publish"
}

apply plugin: "com.github.unafraid.gradle.git-repo-plugin"

repositories {
    jcenter()
    mavenCentral()
    github("RockinChaos", "Repository", "origin", "maven-public")
}
```

![](https://i.imgur.com/vFllc29.png)![](https://i.imgur.com/vFllc29.png)[<img src="https://i.imgur.com/WR5dVKN.png">](https://discord.gg/D5FnJ7C)[<img src="https://i.imgur.com/2YBE4mr.png">](http://ci.craftationgaming.com/)
