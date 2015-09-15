## Getting Started

Gitu is a tiny script for managing multiple git names/emails. It moves `git config --global user.name NAME` and `git config --global user.email EMAIL` to a quick, easy command. Profiles (sets of names and emails) are stored in a yaml file at ~/.git_users.yml.

### Prerequisites
- *nix operating system (Mac OS X or Linux)
- Ruby 2.0.0 or greater

### Installing
`./gitu` should be placed in `/usr/local/bin/` so it can be executed with `gitu`. Use curl or wget for a easiest installation. `~/.git_users.yml` is automatically generated if it doesn't exist the first time any gitu command is run.

#### via curl

`curl -o /usr/local/bin/gitu https://raw.githubusercontent.com/net/gitu/master/gitu && chmod a+x /usr/local/bin/gitu`

#### via wget

`wget -P /usr/local/bin https://raw.githubusercontent.com/net/gitu/master/gitu && chmod a+x /usr/local/bin/gitu`

## Usage

### Profiles

Profiles are named sets of names and emails. Example:

```yaml
github:
  name: net
  email: myemail@me.com
bitbucket:
  name: Atlassian
  email: atlassian@example.com
```

### Commands

#### Set Profile

`gitu [profile]` sets the git global name and email. For example `gitu github` would set the global name and email to the name/email defined under github in `~/.git_users.yml`

#### Current Profile

`gitu` shows the current profile.

#### Set Repository Profile

`gitu -s [profile]` sets the profile for the *current repository*. This adds the name/email to `.git/config` so it stays in effect even after you leave the repository.

#### Add Profile

`gitu + [profile name] [name] [email]` adds a profile. Profiles can also be added directly in `~/.git_users.yml`.

#### Remove Profile

`gitu - [profile name]` removes a profile. Profiles can also be removed directly in `~/.git_users.yml`.

#### Version

`gitu -v` returns the current version.
