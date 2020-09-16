# Mirror Group Memberships

This playbook mirrors local group memberships.

Let's say you have a user, `sally`, on a server. `sally` is a member of some
local groups, but you're not sure which ones.

Now let's say you have two new hires, `frank` and `jen`, and they need to be in
the same groups as `sally`.

Just modify the `vars` section in the playbook like so:

```yaml
  vars:
    user_to_mirror: sally
    users_to_modify:
      - frank
      - jen
```
