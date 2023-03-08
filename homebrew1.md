打开bash_profile

vim ~/.bash_profile

增加如下配置

export http_proxy=http://127.0.0.1:6152
export https_proxy=$http_proxy
alias disproxy='unset http_proxy https_proxy'
变更生效
source ~/.bash_profile
========
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
==> Checking for `sudo` access (which may request your password)...
Password:
==> This script will install:
/opt/homebrew/bin/brew
/opt/homebrew/share/doc/homebrew
/opt/homebrew/share/man/man1/brew.1
/opt/homebrew/share/zsh/site-functions/_brew
/opt/homebrew/etc/bash_completion.d/brew
/opt/homebrew

Press RETURN/ENTER to continue or any other key to abort:
==> /usr/bin/sudo /usr/sbin/chown -R may:admin /opt/homebrew
==> Downloading and installing Homebrew...
HEAD is now at 993768106 Merge pull request #14922 from issyl0/rubocop-naming-method-parameter-name
Warning: /opt/homebrew/bin is not in your PATH.
  Instructions on how to configure your shell for Homebrew
  can be found in the 'Next steps' section below.
==> Installation successful!

==> Homebrew has enabled anonymous aggregate formulae and cask analytics.
Read the analytics documentation (and how to opt-out) here:
  https://docs.brew.sh/Analytics
No analytics data has been sent yet (nor will any be during this install run).

==> Homebrew is run entirely by unpaid volunteers. Please consider donating:
  https://github.com/Homebrew/brew#donations

==> Next steps:
- Run these two commands in your terminal to add Homebrew to your PATH:
    (echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/may/.zprofile
    eval "$(/opt/homebrew/bin/brew shellenv)"
- Run brew help to get started
- Further documentation:
    https://docs.brew.sh

 (echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/may/.zprofile
    eval "$(/opt/homebrew/bin/brew shellenv)"
brew help
Example usage:
