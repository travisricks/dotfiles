#!/usr/bin/env bash

# Close any open System Preferences panes, to prevent them from overriding
# settings we’re about to change
osascript -e 'tell application "System Preferences" to quit'

# Ask for the administrator password upfront
sudo -v

# Keep-alive: update existing `sudo` time stamp until `.macos` has finished
while true; do sudo -n true; sleep 60; kill -0 "$$" || exit; done 2>/dev/null &

echo "Hello $(whoami)! Let's get you set up."

echo "mkdir -p ${HOME}/code"
mkdir -p "${HOME}/code"

printf "TODO:\n\
install: \n\
  Manual Installs from Notion list \n\
\n\
Restart Terminal.app\n\
copy git config from your backup/re-login \n\
run 'pbcopy < ~/.ssh/id_rsa.pub' and paste that into GitHub \n\
copy .npmrc from your backup/re-login \n\
login to literally everything \n\
double check Notion list \n\
"