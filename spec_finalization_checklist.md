* The project team creates a release record as described in https://www.eclipse.org/projects/handbook/#pmi-commands-release
* The project team creates two PRs request against the Jakarta EE Specification Committee specifications repository. The first
PR provides everything requested in the PR template except the javadoc contents. The second PR would include the javadoc contents.
These PRs are intended to provide the items that are required to validate the release, and provide the jakarta.ee website
content for the specification. The github repository to create PRs against is https://github.com/jakartaee/specifications
* The specification committee marks the PR as final when it is ready for voting.
* The project team requests approval for the release from the PMC by sending an email to ee4j-pmc@eclipse.org.
* The project team delivers an IP Log to the IP Team for their review as described in https://www.eclipse.org/projects/handbook/#pmi-commands-iplog
* The project team contacts the EMO to initiate the review by sending an email to emo@eclipse.org.
* The EMO initiates a specification committee ballot by sending an email on the public Jakarta EE Specification Committee
(jakarta.ee-spec@eclipse.org) mailing list that describes the nature of the vote (creation/progress/release) and includes
pointers to the PR request containing the proposed release content (e.g. release review document, specification document, and technical artifacts).
  * A specification committee member votes by responding to the ballot message on the public Jakarta EE Specification Committee mailing list, using the usual +1/0/-1 voting notation.
* On ballot completion
  * the specification PRs are merged by a specification committee representative.
  * the specification staged EFTL TCK is signature is calculated and promoted to the committee download area
  using the https://ci.eclipse.org/jakartaee-spec-committee/job/promote-release/ job.
  * The staged specification api jars are released to maven central by the specification project member who created the staging release.
