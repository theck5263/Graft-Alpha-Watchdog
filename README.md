# Graft-Alpha-Watchdog
Graft SN alpha3 Watchdog/Reset

Copy bcolors.py and snwatchdog.py to your folder of choice ~/supernode/ folder is best.
Copy gn.sh to ~/supernode/BUILD/bin 
	sudo chmod +x gn.sh once in folder
	./gn.sh to launch graftnode reset script once in folder

Copy gs.sh to ~/supernode/
	sudo chmod +x gs.sh once in folder
	./gs.sh to launch graft_server reset script once in folder

These can be run inside seperate TMUX sessions or panes although graftnoded is set for
	--detach so there will be no screen response.

Then run python3 snwatchdog.py inside your script folder, once both above .sh scripts are loaded.

Currently the snwatchdog script looks for only 1 sn "your own" in the sn list and resets both graft instances 
	if this occurs
