## start

```
$ bundle install
$ rake watch # for development
$ rake build # for building (and deployment)
```

## create new project for XXX

- Create new org XXX

### `attachments` repo

- Create attachments repo under XXX org
- Enable Github Pages
- Upload photos
- Get link like https://XXX.github.io/attachments/69.jpg for main photo

### `XXX.github.io` repo

- Fork ann-dau.github.io repo to XXX org
- Rename to `XXX.github.io`
- Git clone https://github.com/XXX/XXX.github.io.git
- Grant Travis-CI to access the new repo https://github.com/settings/connections/applications/f244293c729d5066cf27
- Sync account https://travis-ci.org/profile/wxxeibo and reload page
- Enable `XXX/XXX.github.io`
- Enable `Build only if .travis.yml is present`
- Go to setting, add `PASSWORD` in env vars
- `bundle install` in project dir
- `rake watch` to start dev server
- Change ann-dau in source code to XXX, and commit
  - `_config_localhost.yml`
  - `_config.yml`
  - `gen.sh`
  - `README.md` (include Travis-CI icon)
  - `index.html`
  - `socials.yml`
  - `.travis.yml`
- Run `./gen.sh` to make photo index file
- Restart `rake watch` for changing of `_config_localhost.yml`
- Commit

### google search console

https://www.google.com/webmasters/tools/submit-url

### google analytics

- Create new website
- Update tracking code in `_config.yml`
- Commit

## add new photos

1. Add new photos to attachments repo
1. Push commit
1. Run gen.sh in XXX.github.io repo
1. Push commit
