# metasfresh-maven-repo
Hosts a maven repository for some legacy jars which are no longer available on public maven repositories.
This repo is also referenced from the metasfresh-parent pom

## Important:
* We are in the process of setting up a public maven repo for metasfresh.
* I just imported the artifacts that are hosted here to that new repo. If anyone adds another artifact here, please make sure to also add it to the new repo (or ask [metas-ts](https://github.com/orgs/metasfresh/people/metas-ts))
* if the new nexus server is ready, we will update the metasfresh-parent pom and remove this repo

## Install a new artifact

```
mvn -DlocalRepositoryPath=/path/to/repository_folder install:install-file -Dfile=artifact-1.0.jar -DpomFile=artifact-1.0.pom
```

## Current artifacts and the reason why we have them here
* jms-1.1.jar - the jar itself in not available on maven-ventral: http://central.maven.org/maven2/javax/jms/jms/1.1/
* ftp4che-0.7.1.jar - not available in maven central but available on http://repo.pentaho.org/content/groups/omni/ftp4che/ftp4che/0.7.1/
* pdf-renderer-0.9.0.jar - not available in maven central but available on https://java.net/projects/pdf-renderer/downloads
* jpedal-1.0.jar - not available on maven central
* jp.osdn.ocra-0.2.jar, jp.osdn.ocrb-0.2.1.jar - not available as artifacts in maven central. Fonts were downloaded from http://ansuz.sooke.bc.ca/fonts.php

