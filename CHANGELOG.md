## Changelog
- 3.0.0:
 - Require capistrano 3.7+
 - Implement the plugin system
 - don't fail if puma was already running
 - Added :puma_daemonize option (default is false)

- 2.0.0: 
 - Require puma 3.4+
 - Require Capistrano 3.5+
 - Require capistrano-bundler
 
- 1.2.0: add support for puma user for puma user @mcb & @seuros
- 1.1.0: Set :puma_preload_app to false; Reload Monit after uploading any monit configuration; Always refresh Gemfile @rafaelgoulart @suhailpatel @sime
- 1.0.0: Add activate control app @askagirl
- 0.8.5: Fix smart_restart task to check if puma preloads app
- 0.8.4: Allow patch method (Nginx template) @lonre
- 0.8.2: Start task creates a conf file if none exists @stevemadere
- 0.8.1: Fixed nginx task @hnatt, support for prune_bundler @behe
- 0.8.0: Some changes
- 0.7.0: added Nginx template generator  @dfang
- 0.6.1: added :puma_default_hooks, you can turn off the automatic hooks by setting it false
- 0.6.0: Remove `daemonize true` from default puma.rb file. Explicitly pass `--daemon` flag when needed.
- 0.5.1: Added worker_timeout option
- 0.5.0: Bugs fixes
- 0.4.2: Fix monit template to support chruby
- 0.4.1: Fix puma jungle (debian)
- 0.4.0: Multi-bind support
- 0.3.7: Dependency bug fix
- 0.3.5: Fixed a prehistoric bug
- 0.3.4: I don't remember what i did here
- 0.3.3: Puma jungle start fix
- 0.3.2: Tag option support (require puma  2.8.2+)
- 0.3.1: Typo fix
- 0.3.0: Initial support for puma signals
- 0.2.2: Application pre-loading is optional now (set puma_preload_app to false to turn it off)
- 0.2.1: Tasks are run within rack context
- 0.2.0: Support for puma `ActiveRecord::Base.establish_connection` on
  boot
- 0.1.3: Capistrano 3.1 support
- 0.1.2: Gemfile are refreshed between deploys now
- 0.1.1: Initial support for Monit and configuration override added.
- 0.1.0: Phased restart will be used if puma is in cluster mode
- 0.0.9: puma.rb location changed to shared_path root. puma:check moved to after deploy:check
- 0.0.8: puma.rb is automatically generated if not present. Fixed RVM issue.
- 0.0.7: Gem pushed to rubygems as capistrano3-puma. Support of Redhat based OS for Jungle init script.