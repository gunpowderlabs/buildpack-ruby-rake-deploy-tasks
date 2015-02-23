# Heroku buildpack for running rake db:migrate on deploy

This buildpack is intended for use with [heroku-buildpack-multi], after the regular ruby-buildpack.

# Usage

Append the buildpack-ruby-db-migrate to your buildpack list in the `.buildpacks` file:

```
# ... other buildpacks ...
https://github.com/heroku/heroku-buildpack-ruby
https://github.com/gunpowderlabs/buildpack-ruby-db-migrate
```

# License

MIT, see the LICENSE file.

[heroku-buildpack-multi]:https://github.com/ddollar/heroku-buildpack-multi
[ruby-buildpack]:https://github.com/heroku/heroku-buildpack-ruby
