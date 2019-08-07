# Spec Review Checklist

1. Spec PR
  * PR uses [template](https://github.com/jakartaee/specifications/blob/master/pull_request_template.md)
  * Directory of form {spec}/x.y
  * PDF of form {spec}-spec-x.y.pdf ("-spec" preferred but not required)
  * HTML of form {spec}-spec-x.y.html ("-spec" preferred but not required)
  * Index page {spec}/x.y/_index.md following [template](https://github.com/jakartaee/specification-committee/blob/master/spec_page_template.md)
  * Index page {spec}/_index.md following [template](https://github.com/jakartaee/specification-committee/blob/master/spec_index_template.md)
  * No other files
  * Staging repository link of the form https://oss.sonatype.org/conte/repositories/staging/jakarta/{spec}/jakarta-{spec}-api/x.y.z/
  * EFTL TCK link of the form http://download.eclipse.org/.../*.zip
  * Compatibility certification link of the form https://github.com/eclipse-ee4j/{project}/#{issue}
  * Second PR for just apidocs

2. _index.md
  * Link to spec pdf
  * Link to spec html
  * Link to apidocs
  * Link to final TCK download zip file of the form https://download.eclipse.org/jakartaee/{spec}/x.y/*{spec}-tck-x.y.z.zip
  * Link to API jar file of the form https://search.maven.org/artifact/jakarta.{spec}/jakarta.{spec}-api/x.y.z/jar
  * Name of and link to at least one Compatible Implementation

3. javadocs
  * Footer contains appropriate copyright and link to EFSL license.  This copyright will often be an Eclipse Foundation copyright, even for APIs originally copyrighted by Oracle, but there will be exceptions, and javadoc with other copyright owners.
  * ESFL license is included, usually as doc-files/speclicense.html

4. Spec PDF
  * Correct spec title
  * Version number of the form x.y, not x.y.z
  * Correct Eclipse copyright line
  * No DRAFT or SNAPSHOT

5. Spec HTML
  * Same as PDF

6. TCK zip file
  * README file
  * EFTL license file
  * User's Guide
  * How to test the Compatible Implementation(s) listed in _index.md above with the TCK (may be in UG)

7. TCK User's Guide
  * Software requirements listed
  * Installation and configuration described
  * How to run tests
  * Where to file challenges

8. Compatibility certification request
  * Request follows [template](https://github.com/jakartaee/specification-committee/blob/master/compatibility-certification-request.md)
  * SHA-256 fingerprint matches staged TCK zip file

9. TCK results summary
  * Page is hosted by Compatible Implementation project
  * Includes all information from certification request
  * Summary includes number of tests passed, failed, errors
