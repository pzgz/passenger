# 0.1.0 (3 June 2015)

* BREAKING CHANGES
  * On version of passenger that support both restarting by touch and restarting with passenger-config, the default is to use passenger-config.  set :passenger_restart_with_touch to true to opt out of this.
* Bug fixes:
  * Restored support for CHRuby (@aeons, capistrano/passenger#16)
  * Restored support for passenger installed by bundle (@betesh, capistrano/passenger#10)

# 0.0.5 (12 Apr 2015)

* Bug fixes:
  * When restarting passenger without sudo, made it nevertheless use command map (@betesh, capistrano/passenger#8)
  * We now check whether passenger is installed outside of RVM and use the system installation if it is found.  Otherwise, the user can specify which version of RVM passenger was installed with if it is not the default.

* Command map prefixes for rbenv are automatically added now

# 0.0.4 (26 Mar 2015)

* Bug fixes:
  * rvm:hook task was being called even if it wasn't defined (@betesh, capistrano/passenger#5)

# 0.0.3 (25 Mar 2015)

* Passenger 5 support (@pjkelly, capistrano/passenger#4)

# 0.0.2 (10 Feb 2015)

Bugfixes:
  * If directory doesn't exist, it's created during task (@powertoaster, capistrano/passenger#1)

# 0.0.1 (7 Aug 2014)

Initial release
