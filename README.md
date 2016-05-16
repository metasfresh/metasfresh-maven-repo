# metasfresh-maven-repo
Hosts a maven repository for some legacy jars which are no longer available on public maven repositories

## Install a new artifact

```
mvn -DlocalRepositoryPath=/path/to/repository_folder install:install-file -Dfile=artifact-1.0.jar -DpomFile=artifact-1.0.pom
```

