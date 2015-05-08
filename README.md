# Gitu

Gitu is a very small script for managing multiple git names/emails. It moves `git config --global user.name NAME` and `git config --global user.email EMAIL` to a quick, easy command. Profiles (sets of names and emails) are stored in a yaml file at ~/.git_user

### Prerequisites
- Unix-based operating system (Windows support *may* come later)
- Ruby 2.0.0 or greater

### Installing
./gitu should be placed in `/usr/local/bin/` so it can be run with `gitu`. Use curl or wget for a easiest installation.

#### via curl

`curl -o /usr/local/bin/gitu https://raw.githubusercontent.com/iNety/gitu/master/gitu && chmod a+x /usr/local/bin/gitu`

#### via wget

`wget -P /usr/local/bin https://raw.githubusercontent.com/iNety/gitu/master/gitu && chmod a+x /usr/local/bin/gitu`
