# Specification Plan Review Checklist

After a Specification Committer team notifies the Spec. committee that it intends to begin work on a new specification version a Mentor from the Spec. committee will work with the committer team to create a PR to the Jakarta EE Specification repository that will describe the new release, it's scope, and the plan for development. The checklist here is designed to aid the Specification Committee Mentor as they work with the Committer team to gather and complete the necessary material to hold a successful Plan Review ballot.

Have a committer representative open a new Spec. repository PR for the specification version and paste the following checklist into the PR conversation (comments).

----
1. Spec PR for Plan / Proposal
  - [ ] PR uses [template](https://github.com/jakartaee/specifications/blob/master/pull_request_template.md)
  - [ ] Directory of form {spec}/x.y
  - [ ] (Optional) PDF of form jakarta-{spec}-spec-x.y.pdf ("-spec" preferred but not required)
  - [ ] (Optional) HTML of form jakarta-{spec}-spec-x.y.html ("-spec" preferred but not required)
  - [ ] Index page {spec}/x.y/_index.md following [template](https://github.com/jakartaee/specification-committee/blob/master/spec_page_template.md)
  - [ ] Index page {spec}/_index.md following [template](https://github.com/jakartaee/specification-committee/blob/master/spec_index_template.md)
  - [ ] No other files (e.g., no jakarta_ee_logo_schooner_color_stacked_default.png)

2. _index.md
  - [ ] Link to project PMI plan of the form https://projects.eclipse.org/projects/ee4j.{spec}/releases/x.y/plan
  - [ ] Scope statement changes -- This might be any of
    * Revised specification document, possibly with markup indicating changes
    * Short description of proposed changes
    * List of issues 
        * If many issues are involved consider using an epic (issue of issues) and only provide high-level summary. 
    * If the version update includes a material that are outside the original scope, (i.e. if a feature were to be refactored to another specification or if some major additional functionality is proposed), this should be highlighted.
  - [ ] High level Plan -- If intended to align with a more broad release (i.e. Jakarta EE major release) reference that plan (or plan body). Indicate the milestones intended for *this* specification update (Any planned checkpoints, Feature Complete, Code Complete, TCK Complete, Target Ballot date). 
  - [ ] How to communicate with the Specification committer team (team list, Issue tracker, etc.)
  - [ ] Any additional requirements or details that would be necessary to complete this specification (dependencies, resource requirements, etc.)

3. Proposed Spec PDF (Optional)
  - [ ] Correct spec title, clearly marked preliminary
  - [ ] Correct Eclipse copyright line
  - [ ] Must indicate DRAFT or SNAPSHOT
  - [ ] Correct Logo

4. Proposed Spec HTML (Optional)
  - [ ] Same as PDF

5. TCK
  - [ ] Brief outline describing how TCK will be developed.
  - [ ] Name or list of target implementation partners

6. EMO Requirements 
    TBD
    - [ ] An issue will be created by the EMO to track the release review.
----

## Support and Guidance Resources (Informative)
The mentor should remind the specification committer team of the various process requirements and also the support that is available from the various committees. This can be done via e-mail or a face to face meeting as appropriate.
  - [ ] Pointers to various written resources (such as [Specification Process Guide](https://jakarta.ee/committees/specification/guide/), [TCK Process Guide](https://jakarta.ee/committees/specification/tckprocess/), Eclipse Developement Process, etc.)
  - [ ] Remind the team that the EFSP requires at least one checkpoint update every twelve months. 
  - [ ] Progress Reviews may be required as requested by the Specification committee. 
  - [ ] Remind the team they are obligated to inform the Specification Committee if their work requires evolution to the plan (major features in or out) and/or any significant changes to checkpoint targets.
  - [ ] Remind team of the IP review process for all new, and changes to existing, third party requirements
  - [ ] Remind the team of the community building resources available from the various committees. Some examples
    * Community outreach and involvement through Marketing committee venues and [jakarta.ee](https://jakarta.ee)
        * [What's New, News](https://jakarta.ee/news/)
        * [Community Announcements](https://jakarta.ee/news/?news-type=community_news)
        * [Community Events ](https://jakarta.ee/community/events/)
    * Resource allocation assistance (e.g. additional CI/CD resources anticipated, etc.) from Steering committee
    * General process help from the Specification Committee, etc.)
    * General technical guidance, advice, feedback, review from the Platform Committer team, etc. 
