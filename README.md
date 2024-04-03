# Dotbot APT Plugin

Easily install APK packages with [dotbot](https://github.com/anishathalye/dotbot).

Inspired by:

* [dotbot-apt-get](https://github.com/rubenvereecken/dotbot-apt-get).
* [dotbot-apt](https://github.com/bryant1410/dotbot-apt).

## Usage

Python 3.5+ is needed.

It's easiest to track this plugin in your dotfiles repo:

```bash
git submodule add https://github.com/bernhardrode/dotbot-apk
```

I also recommend having your apk packages list in a separate file since dotbot will need root privileges to use the plugin.
Using the plugin will look something like this:

```bash
sudo ./install -p dotbot-apk/apk.py -c packages.conf.yaml
```

Example `packages.conf.yaml` file:

```yaml
- apk:
  - jq
```

