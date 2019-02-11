Trouble-Shooting
-----------------
The following message was displayed on my screen when I was updating my system:

   Skipping packeges broken dependencies.
   vlc
   vlc-core

The following command help me solved this issue.

  $ sudo dnf install vlc vlc-core --best --allowerasing
