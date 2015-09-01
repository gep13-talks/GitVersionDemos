# GitVersion Demo's
Demo Repository for showing usage of the [GitVersion](https://github.com/GitTools/GitVersion) tool.

## Initial Steps
1. Open Command Prompt
2. Navigate to project folder
3. Initialize new Git Repository
3. Run GitVersion
4. Results in no error, no Git Repository being found
5. Add new file to repository, and commit
7. Run GitVersion
8. Make some changes to the file, add and commit into repository
9. Run GitVersion
10. Discuss what has changed, i.e. the build meta data, which matches the SHA of the commit, and the semantic version, now at +1
11. Make some more changes to the file, add and commit into repository
12. Run GitVersion
13. Discuss the changes again, just to stress the point

## GitFlow Steps - Feature Branch
1. Open SourceTree and point at new repository
2. Initialize GitFlow
3. Run GitVersion
4. Discuss what has changed here, i.e. SHA is still the same, because we are still at the same commit, but logically, things have been added.  Information about where the build is coming from, unstable, also branch information, but it still includes the commit count
5. Create a new feature branch, and make a couple commits into this branch
6. Run GitVersion, and show the continuation of the commit counting, and the addition of the featurea0001 into the NuGet version
7. Close feature branch
8. Run GitVersion

## GitFlow Steps - Release Branch
1. Create a release branch and do some commits
2. Run GitVersion, and highlight the switch to beta
3. Close the release
4. Run GitVersion
5. Discuss the switch to the next minor version, automatically

**NOTE:** Might not do the below, time dependent...

## GitFlow Steps - Hotfix Branch
1. Create a hotfix branch, and do a commit
2. Run GitVersion, and highlight the incremented patch number
3. Close the hotfix
4. Run GitVersion, show that we are still working towards 0.2.0

## GitVersion Init
1. Run GitVersion Init
2. Show how to set up AppVeyor sample scripts
3. Show how to set the next version
4. Remember to save the changes to the file