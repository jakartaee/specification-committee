# Spec Review Checklist

1. Spec PR
  - [ ] PR uses [template](https://github.com/jakartaee/specifications/blob/master/pull_request_template.md)
  - [ ] Directory of form {spec}/x.y
  - [ ] PDF of form jakarta-{spec}-spec-x.y.pdf ("-spec" preferred but not required)
  - [ ] HTML of form jakarta-{spec}-spec-x.y.html ("-spec" preferred but not required)
  - [ ] Index page {spec}/x.y/_index.md following [template](https://github.com/jakartaee/specification-committee/blob/master/spec_page_template.md)
  - [ ] Index page {spec}/_index.md following [template](https://github.com/jakartaee/specification-committee/blob/master/spec_index_template.md)
  - [ ] No other files (e.g., no jakarta_ee_logo_schooner_color_stacked_default.png)
  - [ ] Staging repository link of the form https://jakarta.oss.sonatype.org/content/repositories/staging/jakarta/{spec}/jakarta.{spec}-api/x.y.z/
  - [ ] EFTL TCK link of the form http://download.eclipse.org/.../+.zip
  - [ ] Compatibility certification link of the form https://github.com/eclipse-ee4j/{project}/#{issue}
  - [ ] (Optional) Second PR for just apidocs

2. _index.md
  - [ ] Link to project release plan of the form https://projects.eclipse.org/projects/ee4j.{spec}/releases/x.y/plan
  - [ ] Link to spec pdf
  - [ ] Link to spec html
  - [ ] Link to apidocs
  - [ ] Link to final TCK download zip file of the form https://download.eclipse.org/jakartaee/{spec}/x.y/*{spec}-tck-x.y.z.zip (The folder path is required, the file name pattern is preferred.)
  - [ ] Link to API jar file of the form https://search.maven.org/artifact/jakarta.{spec}/jakarta.{spec}-api/x.y.z/jar
  - [ ] Name of and link to at least one Compatible Implementation

3. javadocs
  - [ ] Footer contains Eclipse copyright and link to license
  - [ ] ESFL license is included, usually as doc-files/speclicense.html
  - [ ] no META-INF directory in PR
  - [ ] javadocs-jar artifact matches apidocs (optional for this release)

4. Spec PDF
  - [ ] Correct spec title
  - [ ] Version number of the form x.y, not x.y.z
  - [ ] Correct Eclipse copyright line
  - [ ] No DRAFT or SNAPSHOT
  - [ ] Correct Logo

5. Spec HTML
  - [ ] Same as PDF

6. TCK zip file
  - [ ] README file (optional for this release)
  - [ ] EFTL license file, preferably named LICENSE.md
  - [ ] User's Guide (or equivalent documentation)
  - [ ] How to test the Compatible Implementation(s) listed in _index.md above with the TCK (may be in UG)

7. TCK User's Guide (or equivalent documentation)
  - [ ] Software requirements listed
  - [ ] Installation and configuration described
  - [ ] How to run tests
  - [ ] Where to file challenges

8. Compatibility certification request
  - [ ] Request follows [template](https://github.com/jakartaee/specification-committee/blob/master/compatibility-certification-request.md)
  - [ ] SHA-256 fingerprint matches staged TCK zip file
  - [ ] Request issue has `certification` label.

9. TCK results summary
  - [ ] Page is hosted by Compatible Implementation project
  - [ ] Includes all information from certification request
  - [ ] Summary includes number of tests passed, failed, errors
  - [ ] SHA-256 fingerprint matches staged TCK zip file on cert request
 
10. Update Jakarta EE API jar
  - [ ] Update the Jakarta EE API jar by submitting a PR to the jakartaee-api project that updates the version number of your API jar file.
