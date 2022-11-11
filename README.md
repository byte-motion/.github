# Shared Workflows for Github Actions


## bytemotion-node-ci
This will create a major, minor, patch, or prerelease after the nodejs repository is successfully built and all tests are passing.
The conditions for each of the afformentioned semantic versions being created and published to npmjs:
- major: An official github release is created
- minor: A pull request has been merged to master
- patch: A commit is made directly to master
- prerelease: An open pull request has a commit pushed to it. The `preid` is `rc`