- [ ] unrar and 7zip installation and paths
- [ ] move hard-coded db credentials to global_ini.py
- [ ] script or doc to add new user to database (can this be a script or manual only?)
- [ ] write deployment.md
- [ ] not in this doc, suggestion: use http://docs.fabfile.org/en/1.10/ to deploy cbr-db


As far as your deployment on linux goes, check out my deployment guide for the flask frontend - you should be aiming at something like that. Technical but not too technical, outline the requirements and the commands to do so (where available), and users should be able to deploy your cbr-db script on their own.

The issue I was having is that there was no mention of test_user and that it's a requirement, you also need to set up your current user to be able to access database without password locally (for the myslq -e "" command for example), same thing with test_user.

You need to install unrar and 7zip-all packages on linux and set their paths instead of the windows location ones. That's also nowhere mentioned.

Other than that the script seem to be showing help message instead of generating output, which is probably something linux related.
