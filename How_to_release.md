# How to release #

  1. Update the change log indicating the date of the release
  1. Switch to Java 8
  1. Run `mvn release:prepare -Prelease`
  1. Run `mvn release:perform -Prelease`
  1. Log in to [Sonatype](https://oss.sonatype.org).
  1. Remove the awaitility-java8-test project so that it's not synced to central
  1. Follow the [Sonatype release directions](https://docs.sonatype.org/display/Repository/Sonatype+OSS+Maven+Repository+Usage+Guide) in bullet 8.
  1. Upload the artifacts to [bintray](http://bintray.com).
  1. Upload the javadoc to googlecode:
    1. Unzip the `awaitility-X-javadoc.jar` into `tags/X/apidocs`
    1. Run `find . -name '*.html' | xargs svn propset svn:mime-type text/html`
    1. Run `find . -name '*.css' | xargs svn propset svn:mime-type text/css`
    1. svn ci -m "Uploading javadocs for version X"
  1. Update the front page and the getting started page.
  1. Send a message to the mailing-list and twitter announcing the new release.

The release is automatically synced to Maven central (the sync process runs hourly).