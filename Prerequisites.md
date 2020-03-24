# X-Code
  1. Open Terminal
  2. Make sure the XCode Developer tools are installed:
  ```
  xcode-select --install
  ```
  This command opens an installation dialog box if needed, or if it's already installed, you see `xcode-select: error: 
  command line tools are already installed, use "Software Update" to install updates` in your Terminal window. Complete the XCode update if needed.

---

# Homebrew
Run the installation command from within the terminal:

``` 
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Example output you see in Terminal:

```
 # Sample Final Output
 ==> Installation successful!

 ==> Homebrew has enabled anonymous aggregate user behaviour analytics.
 Read the analytics documentation (and how to opt-out) here:
   https://docs.brew.sh/Analytics.html

 ==> Next steps:
 - Run `brew help` to get started
 - Further documentation:
     https://docs.brew.sh
```

Verify successful installation by checking the version:
```
 brew -v
```

You see this output, with your version number, as shown:

```
 # Sample Output
 Homebrew 2.2.2
 Homebrew/homebrew-core (git revision 7ac88; last commit 2020-01-02)
 Homebrew/homebrew-cask (git revision 8f0543; last commit 2020-01-02)
```

Homebrew provides access to many standard applications and packages, but isn't optimized for large binary-based applications. As an extension to brew, cask is available. To validate, you can list installed Casks:
```
 brew cask list
```

---

# Python(3.x)

Open a Terminal window and use brew to install Python 3.x.

```
brew install python
```

You should see output like so:

```
 # Sample Final Output
 Python has been installed as
   /usr/local/bin/python3

 Unversioned symlinks `python`, `python-config`, `pip` etc. pointing to
 `python3`, `python3-config`, `pip3` etc., respectively, have been installed into
   /usr/local/opt/python/libexec/bin

 If you need Homebrew's Python 2.7 run
   brew install python@2

 Pip, setuptools, and wheel have been installed. To update them run
   pip3 install --upgrade pip setuptools wheel

 You can install Python packages with
   pip3 install <package>
 They will install into the site-package directory
   /usr/local/lib/python3.6/site-packages

 See: https://docs.brew.sh/Homebrew-and-Python
 ==> Summary
 (brew)  /usr/local/Cellar/python/3.6.5: 4,705 files, 99.5MB
 ```
