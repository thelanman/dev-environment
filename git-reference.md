
### Change Commit Author / Email
Do this if you forgot to set the email / author during commit or don't have it set on global config and need to change commits in past. Also works for commits already pushed to remote origin.
```sh
branch -f --env-filter \
"GIT_AUTHOR_NAME='thelanman'; GIT_AUTHOR_EMAIL='lanahan.j@gmail.com'; \
GIT_COMMITTER_NAME='committed-name'; GIT_COMMITTER_EMAIL='committed-email';" HEAD
```
