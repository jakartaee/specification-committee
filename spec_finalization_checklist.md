* The specification project team creates a release record as described in https://www.eclipse.org/projects/handbook/#pmi-commands-release (if one doesn't already exist)
* The specification project team creates PRs against the [Jakarta EE Specification Committee specifications repository](https://github.com/jakartaee/specifications). The first
PR provides everything requested in the PR template. The javadoc can be included in this first PR, or a second optional PR can be created to only include the javadoc contents.
These PRs are intended to provide the items that are required to validate the release, and provide the jakarta.ee website
content for the specification.
* The specification committee assigns a mentor to the specification PRs to aid with the reviewing and preparation of the specification contents.  Here is an [example mentoring assignment sheet and instructions](https://docs.google.com/document/d/1KaSQBfiyJc2whfQdeuQ1Y7mXnnUnnCuiE-nAqUq5Foo/edit).
* When all review comments have been addressed and approved, the specification committee mentor marks the PR as `final` and ready for `ballot`.
* If a Release Review is required, the specification project team contacts the EMO to initiate the review by sending an email to emo@eclipse.org.
(A Release Review is not required if the current release is a Service Release based on a previously successful Major or Minor
release as indicated by a release record on the project's Releases page, e.g., the [Jakarta Servlet releases page](https://projects.eclipse.org/projects/ee4j.servlet/reviews). A Release Review will not be required for most of the Jakarta EE projects.)
  * An issue will be created by the EMO to track the release review.
  * The specification project team requests approval for the release from the PMC by sending an email to ee4j-pmc@eclipse.org.
  * The specification project team then delivers an IP Log to the IP Team for their review as described in https://www.eclipse.org/projects/handbook/#pmi-commands-iplog.
* The specification committee mentor initiates a specification committee ballot by sending an email on the [public Jakarta EE Specification Committee mailing list](jakarta.ee-spec@eclipse.org) that describes the nature of the vote (creation/progress/release) and includes
pointers to the PR containing the proposed release content (e.g. release review document, specification document, and technical artifacts). See
the [Initiate Ballot Email Template](#initiate-ballot-email-template) section at the end for the template to use.
  * Each specification committee member votes by responding to the ballot message on the public Jakarta EE Specification Committee mailing list, using the usual +1/0/-1 voting notation.
  * The specification committee mentor should monitor the vote and poke the specification committee members if the votes are lagging.
  * (Optional) The specification committee mentor executing the vote may wish to keep tally of the votes in a [spreadsheet such as this](https://docs.google.com/spreadsheets/d/17kIjFbBOuGOv-rQvA3U_MUsNfXAyd8uzPn6h4752tok/edit) -- each component specification has a separate sheet/tab along the bottom.
* On ballot completion
 - [ ] The specification committee mentor adds this final checklist to the main PR.
 - [ ] The specification committee member adds the `approved` label to the PRs, and sends out the Ballot Summary per this [template](#ballot-summary-email-template) to the [public Jakarta EE Specification Committee email list](jakarta.ee-spec@eclipse.org)
  - [ ] The specification committee mentor merges the specification (and apidocs) PRs, ensuring the "date:" field in the _index.md file has an appropriate value to allow publishing.
 - [ ] The specification committee mentor calculates the staged EFTL TCK signature and promotes it to the committee download area
  using the https://ci.eclipse.org/jakartaee-spec-committee/job/promote-release/ job.
 - [ ] The specification project member who created the api staging release promotes the specification api jars to maven central. An example release job script can be found here https://wiki.eclipse.org/MavenReleaseScript.
 - [ ] The specification committee mentor updates the specification page with the ballot results.
This list goes on the committed spec index page.
 - [ ] The specification project team should go through the merged spec website page to verify all the links are valid.
 - [ ] The specification project team should approve the compatibility request.
 - [ ] The compatible implementation project/vendor MUST send an email to tck@eclipse.org for approval of the compatible implementation for trademark usage.
 - [ ] The specification project team should merge any final release branch as appropriate for the branch management for the project.

## Initiate Ballot Email Template

To: Jakarta EE Specification Community Discussions <jakarta.ee-spec@eclipse.org>
 
Subject: BALLOT: Approval to release [SPECIFICATION NAME] [VERSION] 
 
Greetings Jakarta EE Specification Committee.
 
I need your vote to approve and ratify the release of [SPECIFICATION NAME] [VERSION] as part of the Jakarta EE Platform 9 release. 
 
The JESP/EFSP requires a successful ballot of the Specification Committee in order to ratify the products of this release as a Final Specification (as that term is defined in the EFSP). 
 
The relevant materials are available here:
 
[LINKS TO GITHUB PULL REQUESTS]
 
Per the process, this will be a fourteen day ballot, ending on [DATE] that requires a Super-majority positive vote of the Specification Committee members (note that there is no veto). Community input is welcome, but only votes cast by Specification Committee Representatives will be counted.
 
The Specification Committee is composed of representatives of the Jakarta EE Working Group Member Companies (Fujitsu, IBM, Oracle, Payara, Red Hat, Tomitribe, and Primeton), along with individuals who represent the EE4J PMC, Participant Members, and Committer Members.
 
Specification Committee representatives, your vote is hereby requested. Please respond with +1 (positive), 0 (abstain), or -1 (reject).  Any feedback that you can provide to support your vote will be appreciated.

Thanks … 

## Ballot Summary Email Template

To: Jakarta EE Specification Community Discussions <jakarta.ee-spec@eclipse.org>

Subject: BALLOT: Approval to release [SPECIFICATION NAME] [VERSION] 

I declare this ballot complete and approved. The summary of the votes is below. I've marked the corresponding PRs as approved.

The project team and Specification Committee may now engage to complete the release.

Congratulations!

[COPY RESULTS TABLE FROM SPREADSHEET OR OTHER TALLYING MECHANISM]
