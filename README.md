# This is the default menu file for Blackbox 0.33.0 and up
# 
# Lines beginning with the '#' character are ignored.
#
# The new syntax is simpler than the old X resource format...
# Each menu item consists of 2 or 3 fields:
#
#	[command]  (label)  {data}
#
# where [command] is one of:
#
#   [begin] [end] [exec] [exit] [reconfig] [restart]
#   [submenu] [style] [include] [workspaces] [config]
#
# [begin] is used for the top level menu
# [submenu] is used for submenus
# [end] must be used with BOTH [begin] and [submenu] to tell the parser to stop
#   reading from the file.
#
# [exec] (label) {string}
# This will insert an item that runs a program.
#
# [exit] (label)
# This will insert an item that exits the window manager.
#
# [reconfig] (label) {string}
# This will insert an item that tells blackbox to re-read it's configuration
#  files.  {string} is optional, and if supplied, will execute the string with
#  /bin/sh -c before the reconfiguration is performed.  (this is helpful for
#  writing multiple config files and switching between them)
#
# [restart] (label) {string}
# This will insert an item to restart the window manager.  {string} is
# optional, and if omitted, blackbox will restart itself.  If {string} is
# specified, then a different window manager will be started.
#
# [style] (filename)
# This will insert an item to reconfigure blackbox with the new style. This
# change is saved when blackbox exits or restarts.
#
# [include] (filename)
# This will read more menu items from the file "filename".  The file cannot
# contain a [begin] or [end], except for the [end] needed for submenus.
#
# [workspaces] (label)
# This tells Blackbox to insert a "link" to the workspaces menu directly
# into your menu.
#
# [config] (label)
# This tells Blackbox to insert the ConfigMenu into your menu.  The ConfigMenu
# allows you to change several options found in your ~/.blackboxrc file on the
# fly.
#
