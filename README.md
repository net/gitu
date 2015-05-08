## Getting Started

Gitu is a very small script for managing multiple git names/emails. It moves `git config --global user.name NAME` and `git config --global user.email EMAIL` to a quick, easy command. Profiles (sets of names and emails) are stored in a yaml file at ~/.git_users.yml.

### Prerequisites
- Unix-based operating system (Mac OS X or Linux, Windows support *may* come later)
- Ruby 2.0.0 or greater

### Installing
`./gitu` should be placed in `/usr/local/bin/` so it can be executed with `gitu`. Use curl or wget for a easiest installation. `~/.git_users.yml` is automatically generated if it doesn't exist the first time any gitu command is run.

#### via curl

`curl -o /usr/local/bin/gitu https://raw.githubusercontent.com/iNety/gitu/master/gitu && chmod a+x /usr/local/bin/gitu`

#### via wget

`wget -P /usr/local/bin https://raw.githubusercontent.com/iNety/gitu/master/gitu && chmod a+x /usr/local/bin/gitu`

## Usage

### Profiles

Profiles are named sets of names and emails.

```yaml
example:
  name: userone
  email: my.email23@example.com
example2:
  name: usertwo
  email: other.email421@company.com
```

###
