# metasfresh-maven-repo
Hosts a maven repository for some legacy jars which are no longer available on public maven repositories

## Install a new artifact

```
mvn -DlocalRepositoryPath=/path/to/repository_folder install:install-file -Dfile=artifact-1.0.jar -DpomFile=artifact-1.0.pom
```

## Current artifacts and the reason why we have them here
* jms-1.1.jar - link broken on maven central: http://central.maven.org/maven2/javax/jms/jms/1.1/jms-1.1.jar
* ftp4che-0.7.1.jar - not available in maven central but available on http://repo.pentaho.org/content/groups/omni/ftp4che/ftp4che/0.7.1/
* pdf-renderer-0.9.0.jar - not available in maven central but available on https://java.net/projects/pdf-renderer/downloads
* jpedal-1.0.jar - not available on maven central
* jp.osdn.ocra-0.2.jar, jp.osdn.ocrb-0.2.1.jar - not available as artifacts in maven central. Fonts were downloaded from http://ansuz.sooke.bc.ca/fonts.php

