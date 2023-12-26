# puffpuffrack

## The rules

The game goes in phases.  Each phase goes until everyone checks in (there is no time limit, although we should maybe shoot for 1-2 days).  

### Phase 0

Each player commits a patch to that games folder, and an order is specified.  

### Phase n

Each additional phase, each player pulls, opens and modifies the previous track from the player on their right (so the patches move left).  When you're done, you commit your changes, and the phase is over for you.  You may spend as long as needed learning the patch that you received.

### Final Phase

When your original patch gets back to you, add a VCV recorder and perform it.  You may make as many attempts as is needed to perform the patch.  Commit the final wav file to the repo (do not commit mpegs please!).  These files will be gathered and declared to be an album.

### Communication about patches.

All communication about patches must be done in

1) "Notes" modules
2) The git commit message
3) Opening Github Issues

## Git Refresher

PLEASE DO NOT MERGE

To start
```
git clone https://github.com/jvictor0/puffpuffrack.git
```

When your first turn is done

```
git add game_folder/my_file.vcv
git commit -m "My Commit Message"
git pull --rebase origin main
git push origin main
```

To pull the latest changes

```
git pull --rebase origin main
```

## Other Tips

* You can change the framerate if the patch is running too slow.  Try 24khz if the patch won't run.
* You can plug anything into anything.  Nothing bad will happen.
# If the patch won't start, find the audio module and set the output