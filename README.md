# metasfresh-maven-repo
Hosts a public maven repository for some legacy jars which are not or no longer available on maven central.

## usage

Packages placed under `/repository` will get uploaded to the correspondig *github packages* *maven repository* on push
and will be available under: https://maven.pkg.github.com/metasfresh/metasfresh-maven-repo/

:warning: Deleting packages from `/repository` will however not remove them from the *maven repository*.

:warning: Make sure maven coordinates (e.g.  _groupId_ , _artifactId_ ) and the correspondig file names are lower case only.

## Current artifacts
* com.lowagie:itext:2.1.7.js6
* net.sf.jasperreports:jasperreports-functions:6.7.0
* jp.osdn.ocra:jp.osdn.ocra:0.2
* jp.osdn.ocrb:jp.osdn.ocrb:0.2.1
* org.jpedal:jpedal:1.0
* io.github.json-snapshot:json-snapshot-pr:1.0.22
* net.dev.java:pdf-renderer:0.9
* de.metas.report.jasper:montserrat-fonts:jar:8.000
* de.metas.report.jasper:roboto-fonts:jar:2012023.1-2
* de.metas.report.jasper:source-code-pro-fonts:jar:1.0.0
* de.metas.report.jasper:cantarell-fonts:jar:001.001