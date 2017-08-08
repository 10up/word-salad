# word-salad

Word Salad is a simple target for [Crouton](https://github.com/dnschneid/crouton), the Chrome OS chroot system. Targets are config files for Crouton, enabling you to specify exactly how you want to set up your Linux chroot environment. To this end, Word Salad includes:
- nginx as a web server
- php-fpm to handle PHP files
- mysql to handle all your DB needs
- the latest version of WordPress core, fresh from GitHub

Some desired additions in the roadmap are:
- memcache/Redis
- Elasticsearch

# Usage

Word Salad is easy to use. Simply place the target file (targets/wp) somewhere on your Chromebook, install Crouton, and run the following command:
```sudo sh /path/to/crouton -n wp -t core -T /path/to/targets/wp```

Grab a cup of coffee and some avocado toast--installation usually takes 15-20 minutes the first time. Once complete, you'll have a functioning version of available if you navigate to ```http://localhost``` in your browser on your Chromebook.

# Issues

Word Salad is in its very early stages, and we welcome any contributions and pull requests for new features. Eventually, it would be great to see this target added to Crouton itself, so any efforts in that regard (particularly advice around the correct way to pull config files into a Crouton target) would be greatly appreciated.
