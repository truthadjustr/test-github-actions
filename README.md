# Lessons Learned

When you add a repository secret, take note that it is not case-sensive. For
example, adding the secret token key `MySecret` is accessible in the yaml as
`${{ secrets.mysecret }}`. Furthermore, in the github page, the token key is
listed as `MYSECRET` in all-caps.  

### Personal Access Token with repo privileges

So adding secrets is just declaring any variable that can be propagated into
the `env` and can be used in the yaml. This variable has no inherent privileges
attached into them. To create variable values with attached privileges, then 
you must generate `personal access token` with intended attached priviledges
and then add them into `secrets` and by then, the value shall have attached
priviledges which propagates into whatever `action` it is being funnelled into.


### Misc
