# Holiday Hack _Unofficial_ Help & FAQ

# General Help
- **I'm having issues registering or resetting my password** {#generalhelp-registration}
  - Email [support@holidayhackchallenge.com](mailto:support@holidayhackchallenge.com) for assistance
- **It seems like one of the challenges is broken.  Who do I notify?** {#generalhelp-brokenchallenge}
  - First check the Kringle Con status page - https://status2022.kringlecon.com/.  Asking in the Discord channel for that challenge if others are experiencing problems.  You can also @concierge or @moderator to take a look.
- **What if there's a really big problem with a challenge?** {#generalhelp-openissue}
  - You can always DM a concierge or moderator.  You can also open a github issue - https://github.com/CounterHack/HolidayHack2022/issues

# General Technical Help
- **I'm unable to copy/paste in the terminal challenges.  How do I fix this?** {#technicalhelp-copypaste}
  - This behavior is caused by the mouse highlighting text in the tmux session conflicting with wetty.  Below is any ugly fix:
```
# This turns off the mouse within the tmux session (so now wetty can use browser/system mouse to select and copy/paste text), but now you can't select between the top/bottom panes
tmux set -g mouse off

# This binds page up to select the top pane; page down to select the bottom pane
tmux bind-key -T root PageUp select-pane -t 0
tmux bind-key -T root PageDown select-pane -t 1

# To re-enable mouse
tmux set -g mouse on 
```

# Challenges
This is not intended to be hints for the various challenges, but more specific guidance on common technical problems and questions that arise.  If you're looking for a nudge in the right direction, we suggest going to the Discord channel for that challenge.
### 1-a-thing {#challenges-c1t1}
- **Foo**
  - Bar

# Write-ups
- **When can I publish my writeup on my website/github/linkedin?** {#writeups-publish}
  - We kindly ask that you refrain from publicly publishing any answers, write-ups, or walkthroughs until after our submission deadline of January 7, 2022. Once that passes, please feel free to publish!

- **How do I know my writeup has been received?  When will be writeup be reviewed?**
  - The Counter Hack team receives hundreds of submissions, so be patient as they work their way through the backlog.  Candy canes and hot chocolate can only keep fueled for so long before they need to take a break!  :smile: 

- **What are the rules for write-ups?**
  - The general guidelines are 50 pages max and submitted by Jan 7.  If you're looking for some inspiration, you can review previous years winning entries - https://www.holidayhackchallenge.com/past-challenges/

# The More You Know
- **This is my first Holiday Hack Challenge.  Where do I start?**
  - Did you know that multiple previous years are __still__ available? https://holidayhackchallenge.com/past-challenges/