# System Preferences

First thing you need to do, on any OS actually, is update the system! For that:**Apple menu \(\) &gt; About This Mac &gt; Software Update.**

Also upgrade your OS in case you want to work on the latest OS. Sierra is a free upgrade so please check that.

If this is a new computer, there are a couple tweaks you would like to make to the System Preferences. Feel free to follow these, or to ignore them, depending on your personal preferences.

### Users & Groups {#users-groups}

* Login Options -
  &gt;
   Change fast switching user menu to Icon
* Set up Password, Apple ID, Picture, etc.

### Trackpad {#trackpad}

* Point 
  &
   Click
  * Enable Tap to click with one finger
  * Change Secondary click to right corner
  * Uncheck three finger drag
* Scroll 
  &
   Zoom
  * Uncheck all apart from Zoom in and out

### Dock {#dock}

* Visual settings

  * add spaces in dock to separate groups

  * ```
    $ defaults write com.apple.dock persistent-apps -array-add '{"tile-type"="spacer-tile";}'
    $ killall Dock
    ```

* Other settings

  * Remove workspace auto-switching

    ```
      $ defaults write com.apple.dock workspaces-auto-swoosh -bool NO
      $ killall Dock
    ```

### Finder {#finder}

* Toolbar
  * Update to add path, new folder and delete
* Sidebar
  * Add home and code directory
  * Remove shared and tags
  * New finder window to open in the home directory
* View Options
  * Arrange by: Kind
  * Sort by: Name
  * Text Size: 14
  * Select: Use as defaults

### Menubar {#menubar}

* Remove the display and Bluetooth icons
* Change battery to show percentage symbols

### Spotlight {#spotlight}

* Uncheck fonts, images, files etc.
* Uncheck the keyboard shortcuts as we'll be replacing them with Alfred.

### Accounts {#accounts}

* Add an iCloud account and sync Calendar, Find my mac, Contacts etc.

#### Update Homebrew formulae: {#update-homebrew-formulae-}

```
$ brew update
```



