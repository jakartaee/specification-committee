# Specification Progress Review Checklist

From time to time the Specification Committee may request that specification project committer teams submit material for a Progress Review ballot. 
This checklist is for the Mentor to help the committer team gather and organize that material. 
The JESP requires all specification projects submit a progress review every twelve (12) months.
Once the material is collected and ready (either in a PR, or the mentor simply receives confirmation that the original plan is still valid) 
the mentor will start a Progress Review ballot. 
This check-list assumes that the previous ballots necessary to get to this state have been successful and material from those events is available. 
The mentor is not responsible for gathering this material and is not responsible for assessing progress in any way.

If the Specification committee has requested specific information, the mentor should be sure to convey this request to the committer team. 
The mentor should review the materials provided for the Progress Review to ensure that the questions raised for the progress review have been addressed. 
If the progress review is purely procedural (i.e. it's been twelve months or more since the last ballot) then all that is needed is to confirm that 
the plan as previously agreed, is still valid and that checkpoint artifacts (Milestone builds, TCK updates, etc.) previously agreed to have been produced.

A pre-ballot PR may not be required if there are no changes to the plan or scope, from the previously approved plan review/proposal. 
If a pre-ballot PR is needed (for example if the plan or scope needs to be updated), that material will be included in the 
Progress Review ballot notice and likely a PR will have to be generated to reflect these updates.

----
1. Spec PR for Plan / Proposal
  - [ ] There is no new material that wasn't previously provided that would impact the existing Specification "work in progress" page layout.

2. _index.md
  - [ ] If there are milestones previously approved and/or documented on the Specification page, but now out of date, or not feasible (missed checkpoints or other milestones), there must be a proposed PR to refresh the previously approved plan material.
  - [ ] The progress review should demonstrate the agreed plan is still correct and accurate. If it is not, the Progress Review is an opportunity to revise the plan as needed.
  - [ ] Mentor to confirm (via consultation with committer team) the scope is correct. If it has been revised, those changes should be summarized. Regardless, the committer team is responsible for providing any statements or documentation describing progress for the progress review materials.
    - [ ] The mentor may wish to review the Plan Review Ballot checklist to confirm all items are captured. 
    - [ ] If checkpoint or scope material is derived from issues or epic issues, the mentor may wish to request the committer team provide a summary statement of the specific progress against the issue or issues. 
    - [ ] The committer team should provide an overall assessment that confirms they are "on track" or produces a plan revision that reflects the evolution since the last ballot. 
  - [ ] The mentor should focus material for this review on progress of this specification revision and not the progress or changes associated with higher level projects (i.e. it is probably insufficient to say "schedule changed in Platform Release Plan so we're changing too"). Scope changes that have been imposed on this specification may certainly be noted and may be a source for plan revisions.
  - [ ] Any changes or additional requirements, resource needs (e.g. CI/CD resources), feature changes, etc. should be reflected in the specification plan revision. If there are no changes the committer team should be able to demonstrate that they are progressing within the original plan that is already approved.

3. Proposed Spec PDF (Optional)
  - [ ] Correct spec title, clearly marked preliminary
  - [ ] Correct Eclipse copyright line
  - [ ] Must indicate DRAFT or SNAPSHOT
  - [ ] Correct Logo

4. Proposed Spec HTML (Optional)
  - [ ] Same as PDF

5. TCK
  - [ ] Some statement or evidence of TCK development progress and accomplishment from previous review

6. EMO Requirements 

    N/A
    
----
When the mentor is satisfied that the material listed above is gathered and up to date, they will initiate a Progress Review ballot. See below for sample ballot notice/request.

If the ballot is successful, the ballot results will be added to the Specification page to memorialize that this event occurred.

If the progress review ballot fails, the project would need to be referred to the Specification Commitee for further action and next steps.

A sample ballot conclusion e-mail is included below.

----
Sample Progress Review Ballot e-mail Notification

    To: Jakarta EE Specification Community Discussions jakarta.ee-spec@eclipse.org
    
    Subject: BALLOT: Progress Review [SPECIFICATION NAME] [VERSION]

    Greetings Jakarta EE Specification Committee.

    I need your vote to approve the progress review materials of 
    [SPECIFICATION NAME] [VERSION].
    
    The JESP/EFSP requires progress every twelve months or as requested 
    by the Specification Committee.

    The relevant materials are available here:

    [LINKS TO GITHUB PULL REQUESTS or other summary documentation]

    Per the process, this will be a fourteen (14) day ballot, ending on [DATE]
    that requires a Super-majority positive vote of the Specification
    Committee members (note that there is no veto). 
    Community input is welcome, but only votes cast by Specification Committee Representatives will be counted.

    The Specification Committee is composed of representatives of the 
    Jakarta EE Working Group Member Companies (Fujitsu, IBM, Oracle, 
    Payara, Tomitribe, Primeton, and Shandong Cvicse Middleware Co.), 
    along with individuals who represent the EE4J PMC, Participant 
    Members, and Committer Members.

    Specification Committee representatives, your vote is hereby requested. 
    Please respond with +1 (positive), 0 (abstain), or -1 (reject). 
    Any feedback that you can provide to support your vote will be appreciated.

    Thank you,
    [Mentor Name]

----

Ballot Summary Email Template

    To: Jakarta EE Specification Community Discussions jakarta.ee-spec@eclipse.org
    
    Subject: BALLOT RESULTS: Progress Review [SPECIFICATION NAME] [VERSION]
  
    I declare this ballot complete and [approved/failed]. 
    The summary of the votes is below. I've marked the corresponding PRs 
    as approved.

    Thank you,
    [Mentor Name]

    [COPY RESULTS TABLE FROM SPREADSHEET OR OTHER TALLYING MECHANISM]
