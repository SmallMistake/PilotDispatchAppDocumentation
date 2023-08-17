# Using our Gitflow

## Overview 
This repository uses a Gitflow cycle to ensure that merges are safe and always have production ready code. Individual development should not be done on the main stable development branches

<img style="background-color:white" src="./images/uz_gitflow.png" alt="Gitflow Example">

<blockquote>
<strong>Branch Types</strong>
<pre>
    - <strong>Release_Branch</strong>: This is the current version that is out in the stores.
        - Only the Stable_Development_Branch should merge into it.
    - <strong>Stable_Development_Branch</strong>: This is the internal devoplment branch that includes commits of stable new features
        - When ready to release to stores, merge into Release_Branch
    - <strong>Feature_Branch</strong>: Created off of the Stable_Development_Branch each time a developer starts to work on a new feature
        - Merge into the Stable_Development_Branch when ready
    - <strong>Previous_Release_Branch</strong>: If it is seen as important that a backup should be made of an important version of the releaase branch is merged into it. 
        Create this branch off of the Release branch
</pre>
</blockquote>


## Workflow
1) Create a feature branch off of the Stable_Development_Branch.
2) Do your work on the feature branch
3) Create a pull request to merge your changes into the Stable_Development_Branch
4) When a store release is ready to be made, create a pull request to merge the Stable_Development_Branch into the Release_Branch
5) Create a release Branch for the new version if desired to keep the code for posterities sake.