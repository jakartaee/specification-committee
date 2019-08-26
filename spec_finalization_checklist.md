* The project team creates a release record as described in https://www.eclipse.org/projects/handbook/#pmi-commands-release
* The project team creates two PRs request against the Jakarta EE Specification Committee specifications repository. The first
PR provides everything requested in the PR template except the javadoc contents. The second PR would include the javadoc contents.
These PRs are intended to provide the items that are required to validate the release, and provide the jakarta.ee website
content for the specification. The github repository to create PRs against is https://github.com/jakartaee/specifications
* The specification committee marks the PR as final when it is ready for voting.
* Create a release record as described in https://www.eclipse.org/projects/handbook/#pmi-commands-release
* If a Release Review is required, the project team contacts the EMO to initiate the review by sending an email to emo@eclipse.org.
(A Release Review is not required if the current release is a Service Release based on a previously successful Major or Minor
release as indicated by a release record on the project's Releases page, e.g., the [Jakarta Servlet releases page](https://projects.eclipse.org/projects/ee4j.servlet/reviews). A Release Review will not be required for most of the Jakarta EE projects.)
  * An issue will be created by the EMO to track the release review
  * The project team requests approval for the release from the PMC by sending an email to ee4j-pmc@eclipse.org.
  * The project tream then delivers an IP Log to the IP Team for their review as described in https://www.eclipse.org/projects/handbook/#pmi-commands-iplog.
* The EMO initiates a specification committee ballot by sending an email on the public Jakarta EE Specification Committee
(jakarta.ee-spec@eclipse.org) mailing list that describes the nature of the vote (creation/progress/release) and includes
pointers to the PR request containing the proposed release content (e.g. release review document, specification document, and technical artifacts).
  * A specification committee member votes by responding to the ballot message on the public Jakarta EE Specification Committee mailing list, using the usual +1/0/-1 voting notation.
* On ballot completion
  * the designated specification committee representative adds this final checklist to the main PR.
  * the specification committee representative merges the specification PRs.
  * the designated specification committee representative calculates the staged EFTL TCK is signature and promotes it to the committee download area
  using the https://ci.eclipse.org/jakartaee-spec-committee/job/promote-release/ job.
  * The specification project member who created the staging release promotes the specification api jars to maven central.
  * The EMO updates the specification page with the ballot results.
this list goes on the committed spec index page.
  * The project team should go through the spec merged website page to verify all the links are valid.
* Post ballot completion, EMO asks webmaster to push changes to jakarta.ee
