# git-subrepo 
Git Subrepo is a bit like git submodules but it is a implementation with focus on total integration and adoption.

The Git SubRepo pattern is designed to form a single Global Repositiory with Authoritiv Permissions. 
So it is not designed mainly to update existing sources in the repositorys that it clones.

It Can! But the flow is optimized as sayed to be Authoritiv that means the source repo gets used
to ingest changes if needed and apply own changes to it. So it is mainly the core driver
of our Distributed world wide build grid. As that is not designed to contribute back while still
ingesting changes from legacy git repositorys. 

In case that you want to add multiple branches you would do the following pattern

git subrepo clone source target/branches/name

most optimal you will not need to do so often when the project is table or in shape but as we are developers
we maybe need such patterns to migrate so i want to give white glove greenfild patterns to do so

when the branch is not needed any more you simple remove the directory like you would remove a branch
thats it.

.subrepo files are meta files and do not need to get touched manual they get used by tooling most of the time
only touch them if you know what your doing. in case of source contribution so pushes back to the source
this file gets always excluded so do not worry about it.
