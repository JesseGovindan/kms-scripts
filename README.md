IMPORTANT!

Please add the following line somewhere in your .bashrc file. (usually located in your home directory)

```export PATH=~/kms-scripts:$PATH```
Be sure to change the path to the path where you have cloned this repo on your machine


Also export the following variable
```EXPORT KINESIS_ROOT=~/Projects/kinesis/ # Change this to your actual directory```

# tag-kinesis-repo
This script finds the next patch version tag number for a repo, then creates and pushes a new tag.
It may be used as a standalone tool but is better off used as a starting point for creating scripts for tagging your
repos.

Usage tag-kinesis-repo "your-repo-folder-name" "tag-version-prefix"

i.e ```tag-kinesis-repo "kms" "qa5."```

To help figure out what the appropriate tag-version-prefix should be, use the latest-tag script.

# latest-tag
Finds the next patch version (or last set of numbers after a fullstop) in a repo by examining the current set of tags
and attempting to parse a 
