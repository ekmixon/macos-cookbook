# macOS Cookbook

[![Build Status](https://dev.azure.com/office/OE/_apis/build/status/Microsoft.macos-cookbook?branchName=master)](https://dev.azure.com/office/OE/_build/latest?definitionId=5072&branchName=master)

Chef resources and recipes for managing and provisioning macOS.

- [Chef Requirements](#chef-requirements)
- [Supported OS Versions](#supported-os-versions)
- [Attributes](#attributes)
- [Recipes](#recipes)
- [Data Bags](#data-bags)
- [Resources](#resources)

## Officially Supported Chef Versions

- Chef 16
- Chef 17

## Supported OS Versions

- macOS High Sierra 10.13
- macOS Mojave 10.14
- macOS Catalina 10.15
- macOS Big Sur 11.0

## Attributes

### Admin User and Password

```ruby
node['macos']['admin_user'] = 'vagrant'
node['macos']['admin_password'] = 'vagrant'
```

Each of these attributes defaults to vagrant since our resources are developed
with the Vagrant paradigm. In other words, the user and password declared here
should be an admin user with passwordless super-user rights.

## Resources

- [`automatic_software_updates`](https://github.com/Microsoft/macos-cookbook/blob/master/documentation/resource_automatic_software_updates.md)
- [`certificate`](https://github.com/Microsoft/macos-cookbook/blob/master/documentation/resource_certificate.md)
- [`command_line_tools`](https://github.com/Microsoft/macos-cookbook/blob/master/documentation/resource_command_line_tools.md)
- [`keychain`](https://github.com/Microsoft/macos-cookbook/blob/master/documentation/resource_keychain.md)
- [`macos_user`](https://github.com/Microsoft/macos-cookbook/blob/master/documentation/resource_macos_user.md)
- [`plist`](https://github.com/Microsoft/macos-cookbook/blob/master/documentation/resource_plist.md)
- [`remote_management`](https://github.com/Microsoft/macos-cookbook/blob/master/documentation/resource_remote_management.md)
- [`spotlight`](https://github.com/Microsoft/macos-cookbook/blob/master/documentation/resource_spotlight.md)
- [`xcode`](https://github.com/Microsoft/macos-cookbook/blob/master/documentation/resource_xcode.md)
