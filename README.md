## Deprecated

This buildpack is deprecated.

If you need to run a task after you build but before you deploy please [use Release phase](https://devcenter.heroku.com/articles/release-phase).

If you need to modify files on disk (which release phase will not do). You can hook into the `assets:precompile` task

```ruby
# Rakefile
task "assets:precompile" do
  Rake::Task["assets:precompile"].invoke
  # Run your custom code here
end
```
