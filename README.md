# Lessons Learned

When you add a repository secret, take note that it is not case-sensive. For
example, adding the secret token key `MySecret` is accessible in the yaml as
`${{ secrets.mysecret }}`. Furthermore, in the github page, the token key is
listed as `MYSECRET` in all-caps.  

# Environment Variable
