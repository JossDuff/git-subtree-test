# git-subtree-test

Playing around with git subtrees

`git subtree add --prefix=optimism https://github.com/ethereum-optimism/optimism.git develop --squash`

`git subtree merge -P optimism --squash <commit hash>`

Enabling fetching of new commits (and referencing branches & tags!):
`git remote add <dependency name> <git url>`

fetching changes from that remote:
`git fetch <dependency name>`

merging in new changes example:
`git subtree merge -P git-subtree-test-dependency --squash git-subtree-test-dependency/main`
(via tag)
`git subtree merge -P git-subtree-test-dependency --squash tags/<tag-name>`
