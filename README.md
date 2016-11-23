
# DEPRECATED

Please don't use this ad-hoc repository anymore. Instead, feel free to use our public maven repository at  https://repo.metasfresh.com/content/groups/mvn-public/.

Note that the new repository is also wired into our [metasfresh-parent](https://github.com/metasfresh/metasfresh-parent) `pom.xml`, so in most cases, you don't need to change anything. 

sidenote: to find out how to build metasfresh for yourself, you can take a look at our [developer documentation](http://docs.metasfresh.org/pages/developers/index_en).

# metasfresh-maven-repo
Hosts a maven repository for some legacy jars which are no longer available on public maven repositories.
This repo is also referenced from the metasfresh-parent pom

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

