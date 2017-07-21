Basic premise: interact with repos/orgs as if they were a filesystem

Top-level command: om

Do things like:

```shell
$ cd ~/Orgs/MyOrg
$ om repos

Repositories in MyOrg:
- foo       [public]  [local: master]
- bar       [private] [local: other-branch]
- baz       [public]

$ om people

Members of MyOrg:
- @sara   Sara Watkins
- @bob    Bob Sellers

$ om people add --collaborator @danny

Added @danny as an outside collaborator to MyOrg

$ om people --invites

Pending invitations to MyOrg:
- @bill   Bill Wong

$ om people --members --data "username,email"
sara,sara@watkins.org
bob,bob@sellers.com

$ om teams

Teams in MyOrg:
- Design
- DevOps
- UI/UX
- Backend
- Marketing
```
