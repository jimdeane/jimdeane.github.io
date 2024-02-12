- Manual Testing done.
  - Work tested locally.
  - Tested on Web AND Mobile
  - Feature branch deployed to DEV and tested by assignee.
  - Depending on complexity or uncertainty, invite colleague for screen share and walk through.
     - Alternatively send a link and ask colleague to run through.
     - This saves time as it is more expensive to change something after merged to MAIN.
  - Favour team communication over processes. 
    - Better to jump on a call (or group chat) and resolve an issue or uncertainty.
- Automated Tests updated.
  - Unit Tests with code coverage not below [%].
  - Integration Tests.
  - If we have a recurring bug in UAT/PRD, we are probably missing a test.
- Documentation updated.
  - README file.
  - Any diagrams in [Shared Location].
- PR opened and reviewed and approved by colleague
  - This doesn't replace a code review, will schedule code reviews to look at solution as a whole.
  - PR automated build passes.
- If big or infrastructure changes were made it would be a good idea to kick off a full build (all components) for your feature.
- Deploy feature to DEV and confirm successful before merging.
- Merge PR into MAIN
  - Please use Squash Merge, unless you worked on 2 stories and want to retain separate commits.
    - In this case probably do a local squash to end up with 2 respective commits.
  - Consider deleting feature branch on github (you still have local branch if needed)
  - Merging into MAIN will kick off a FULL automated build of all components. It is the developer's responsibility to check if succeed.
- Create a release of artefact from MAIN and deploy to DEV.
  - @<3B5C44BC-92BA-6D9F-826D-926A68021628>, @<D31469F5-91ED-6A8D-9405-745A1E05A07A>  to look at automating this step.
  - Share link on group chat as candidate for UAT then PRD.
    - This is important since we are all working async, @<D240661F-A317-6553-A161-6D2B6F25387D> can then just pick up latest Release and promote to UAT.




