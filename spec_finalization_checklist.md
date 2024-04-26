* The specification project team creates a release record as described in https://www.eclipse.org/projects/handbook/#pmi-commands-release (if one doesn't already exist)
* The specification project team creates PRs against the [Jakarta EE Specification Committee specifications repository](https://github.com/jakartaee/specifications). The first
PR provides everything requested in the PR template. The javadoc can be included in this first PR, or a second optional PR can be created to only include the javadoc contents.
These PRs are intended to provide the items that are required to validate the release, and provide the jakarta.ee website
content for the specification.
* The specification committee assigns a mentor to the specification PRs to aid with the reviewing and preparation of the specification contents.  Here is an [example mentoring assignment sheet and instructions](https://docs.google.com/document/d/1KaSQBfiyJc2whfQdeuQ1Y7mXnnUnnCuiE-nAqUq5Foo/edit).
* When all review comments have been addressed and approved, the specification committee mentor marks the PR as `final` and ready for `ballot`.
* The specification committee mentor initiates a specification committee ballot by sending an email on the [public Jakarta EE Specification Committee mailing list](jakarta.ee-spec@eclipse.org) that describes the nature of the vote (creation/progress/release) and includes
pointers to the PR containing the proposed release content (e.g. release review document, specification document, and technical artifacts). See
the [Initiate Ballot Email Template](#initiate-ballot-email-template) section at the end for the template to use.
  * Each specification committee member votes by responding to the ballot message on the public Jakarta EE Specification Committee mailing list, using the usual +1/0/-1 voting notation.
  * The specification committee mentor should monitor the vote and poke the specification committee members if the votes are lagging.
  * (Optional) The specification committee mentor executing the vote may wish to keep tally of the votes in a [spreadsheet such as this](https://docs.google.com/spreadsheets/d/17kIjFbBOuGOv-rQvA3U_MUsNfXAyd8uzPn6h4752tok/edit) -- each component specification has a separate sheet/tab along the bottom.
* On ballot completion, the specification committee mentor:
 - [ ] adds this final checklist to the main PR.
 - [ ] adds the `approved` label to the PRs, and sends out the Ballot Summary per this [template](#ballot-summary-email-template) to the [public Jakarta EE Specification Committee email list](jakarta.ee-spec@eclipse.org)
 - [ ] calculates the staged EFTL TCK signature and promotes it to the committee download area
  using the https://ci.eclipse.org/jakartaee-spec-committee/job/promote-release/ job. Manually editing the jenkins Build Information will help identify the build (ie. Mail 2.0 or CDI 3.0).
 - [ ] merges the specification (and apidocs) PRs, ensuring the "date:" field in the _index.md file has an appropriate value to allow publishing.
 - [ ] updates the specification page with the ballot results. This is normally done via a separate PR that should be reviewed, approved, and merged.
 - [ ] notifies the EMO of the ballot results by email to [emo@eclipse-foundation.org](emo@eclipse-foundation.org). Just forward the ballot summary note sent earlier to the public Spec Committee email list.
 - [ ] creates an issue in the specification project that includes the following checklist for the specification project team:
 \<include url of Issue here>

<!-- Add this list to the specification project issue.  Delete this section of checklist from Spec PR once this specification project issue is created and logged. -->
 ----
 - [ ] promotes api staging release promotes the specification api jars to maven central. An example release job script can be found here https://wiki.eclipse.org/MavenReleaseScript.
 - [ ] go through the merged jakarta.ee specification website page to verify all the links are valid.
 - [ ] if XML Schemas are published on https://jakarta.ee/schemas, send a PR to update the status from `Draft` to `Final`.
 - [ ] approve the compatibility request.
 - [ ] merge any final release branch as appropriate for the branch management for the project.

## Initiate Ballot Email Template

To: Jakarta EE Specification Community Discussions <jakarta.ee-spec@eclipse.org>
 
Subject: BALLOT: Approval to release [SPECIFICATION NAME] [VERSION] 
 
Greetings Jakarta EE Specification Committee.
 
I need your vote to approve and ratify the release of [SPECIFICATION NAME] [VERSION] as part of the Jakarta EE Platform 11 release. 
 
The JESP/EFSP requires a successful ballot of the Specification Committee in order to ratify the products of this release as a Final Specification (as that term is defined in the EFSP). 
 
The relevant materials are available here:
 
[LINKS TO GITHUB PULL REQUESTS]
 
Per the process, this will be a fourteen day ballot, ending on [DATE] that requires a Super-majority positive vote of the Specification Committee members (note that there is no veto). Community input is welcome, but only votes cast by Specification Committee Representatives will be counted.
 
The Specification Committee is composed of representatives of the Jakarta EE Working Group Member Companies (Fujitsu, IBM, Oracle, Payara, Tomitribe, Primeton, and Shandong Cvicse Middleware Co.), along with individuals who represent the EE4J PMC, Participant Members, and Committer Members.
 
Specification Committee representatives, your vote is hereby requested. Please respond with +1 (positive), 0 (abstain), or -1 (reject).  Any feedback that you can provide to support your vote will be appreciated.

Thanks … 

## Ballot Summary Email Template

To: Jakarta EE Specification Community Discussions <jakarta.ee-spec@eclipse.org>

Subject: BALLOT: Approval to release [SPECIFICATION NAME] [VERSION] 

I declare this ballot complete and approved. The summary of the votes is below. I've marked the corresponding PRs as approved.

The project team and Specification Committee may now engage to complete the release.

Congratulations!

[COPY RESULTS TABLE FROM SPREADSHEET OR OTHER TALLYING MECHANISM]
