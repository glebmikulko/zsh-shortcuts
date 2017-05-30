# zsh-shortcuts
## rails

**Maintainer:** [robbyrussell](https://github.com/robbyrussell)

#### rails aliases:
| Alias | Command                  |
|:------|:-------------------------|
| _rc_  | rails console            |
| _rd_  | rails destroy            |
| _rdb_ | rails dbconsole          |
| _rg_  | rails generate           |
| _rgm_ | rails generate migration |
| _rp_  | rails plugin             |
| _ru_  | rails runner             |
| _rs_  | rails server             |
| _rsd_ | rails server --debugger  |

#### rake aliases:
| Alias   | Command                       |
|:--------|:------------------------------|
| _rdm_   | rake db:migrate               |
| _rdms_  | rake db:migrate:status        |
| _rdr_   | rake db:rollback              |
| _rdc_   | rake db:create                |
| _rds_   | rake db:seed                  |
| _rdd_   | rake db:drop                  |
| _rdtc_  | rake db:test:clone            |
| _rdtp_  | rake db:test:prepare          |
| _rdmtc_ | rake db:migrate db:test:clone |
| _rlc_   | rake log:clear                |
| _rn_    | rake notes                    |
| _rr_    | rake routes                   |
---

## bundler

**Maintainer:** [robbyrussell](https://github.com/robbyrussell)

Enables aliases to [Bundler](http://gembundler.com/).

| Alias | Description                                                 |
|:------|:------------------------------------------------------------|
| be    | Bundle exec, execute a command in the context of the bundle |
| bi    | Bundle install                                              |
| bu    | Bundle update                                               |

Also creates shell aliases so you don't have to type "bundle exec" before most common ruby commands when you are in a directory with a Gemfile. Here is a [list of commands](https://github.com/robbyrussell/oh-my-zsh/blob/master/plugins/bundler/bundler.plugin.zsh#L9) it does this for: `annotate cap capify cucumber ey foreman guard heroku middleman nanoc rackup rainbows rails rake rspec ruby shotgun spec spork thin thor unicorn unicorn_rails`

---
## rvm

| Command         | Description                                                                                                                                     |
|:----------------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| _rb18_ [GEMSET] | shortcut for `rvm use ruby-1.8.7-p334@GEMSET` (with gemset completion)                                                                          |
| _rb19_ [GEMSET] | shortcut for `rvm use ruby-1.9.2-p180@GEMSET` (with gemset completion)                                                                          |
| _rubies_        | list installed rubies                                                                                                                           |
| _gemsets_       | list gemsets for currently active ruby                                                                                                          |
| _gems_          | list gems available in currently active gemset **Note: This has opinions about colors. It should be re-factored to be customizable in themes.** |

After `rvm-update` (alias for `rvm get head; rvm reload`), run `rvm-link-completion` to make a symlink to the official zsh completion file that comes with rvm into your oh-my-zsh rvm plugin directory.

