# Notes
### Change name branch
```
git branch -m old_branch new_branch         # Rename branch locally    
git push origin :old_branch                 # Delete the old branch    
git push --set-upstream origin new_branch   # Push the new branch, set local branch to track the new remote
```
### Copy database from staging to production on heroku
`heroku pg:backups capture --app STAGING`

`heroku pg:backups restore $(heroku pg:backups public-url --app PRODUCTION) --app STAGING`
