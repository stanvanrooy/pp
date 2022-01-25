### Do you find any evidence that developers ship software they know isn't perfect?
- GitHub actions -> GH actions was initially shipped with a rather
  limited feature set. Even now, 2 years later, there are still 
  some pretty 'basic' features missing. But it still works _good enough_
  for us.
- Microsoft Teams -> Widely used even though it's horrendously slow,
  crashes relatively often and has countless other bugs. It's far from
  perfect, but it's still _good enough_.

### Will it take more time to deploy a tightly coupled monolith, or loosely coupled micro services?
First guess: the monolith will take longer to deploy.

__Deploying a monolith__
+ Should be simple to deploy: one click on the button;
- Deployments/builds are (a lot) slower, even for relatively small
  changes;
- Because builds are slower, TTR is also slower;
- Since all changes need to tested, the DLT is longer;

__Deploying micro services__
+ Builds are fast, so are deployments;
- Because builds are faster, TTR is also faster;
+ Changes are small & local, so the DLT is shorter;
- Deployments can become harder to set up & manage;

### Can you think of software that suffers from 'feature bloat'?
__Azure DevOps__
Everything you can think of, is available in Azure DevOps,
but most of that we never use. I think a lot of it is legacy, that is
still needed for backwards compatibility.

__Microsoft Teams__
This is both a plus and a min. For 'normal' MS Teams users, a lot of the
functionality is not ever needed. It just complicates the UI and the
user experiences. _But_, for the few power horses it is an absolute game
changer, to collaborate in Excel, give presentations using PowerPoint,
keep track of to-do's in ToDo and use the integration with Jira &
Salesforce for tracking projects.

#### Glossary
- DLT -> delivery lead time: the amount of time that goes from the commit
  to the release in production.
- TTR -> time to restore: how much time is needed to recover from
  downtime introduced with a release.

