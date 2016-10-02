# Easy-WI ARK Mod / Content Manager

<h3>This is a ARK Mod / Content Manager for the www.Easy-WI.com Webinterface.</h3>

---

<h4>Requirements:</h4>
- Debian 8 or higher, Ubuntu 16 or higher
- Root User
- curl
- wget
- sudo

---

<h4>Which functions are available in Ark Mod Manager?</h4>

- Install a single ARK Mod ID
- Install predefined ARK Mods (IDs are inside the "ark_mod_downloader.sh" Script)
- Update all installed ARK Mods IDs
- Install Updater Script + Cronjob (for automatically Update) (in Progress)
- Uninstall Updater Script + Crontab (in Progress)
- Remove a single ARK Mod ID
- Remove all ARK Mod IDs

---

<h4>Which Script is what?</h4>

For install, update or remove from Mod IDs, have i the ark_mod_manager.sh written.
Inside this script are all functions, what you are looking for.</br>
Only for Update per Cronjob/Crontab have i the ark_mod_updater.sh written.

---

<h4>What must I edit befor it's running?</h4>

Edit inside the two Scripts the Masteruser with your Masterserver Webinterface User, who's you in installing has given.
Place the two Scripts inside your Root directory and copy following in your Terminal (Putty or what ever):
chmod 700 ./ark_mod_updater.sh && chmod 700 ./ark_mod_manager.sh && ./ark_mod_manager.sh

Inside the Updater Script have you the Option, to retrive an E-Mail on Failure.
Change the E-Mail Field to your E-Mail Address to activate this Option.

---

<h4>How works the Updater per Cronjob?</h4>

Open your console (Putty/WinSCP or what you use) and paste this into:</br>
echo "30 1 * * * /root/ark_mod_updater.sh >/dev/null 2>&1" >> /etc/cron.d/ark_mod_updater && service cron restart

---

<h4>How does the support work?</h4>

I give only in Github Support. No Private or another way are supported!

