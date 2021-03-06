# Scheme environment

This will be a simple Scheme implementation switcher.

# How to install

```
$ curl https://raw.githubusercontent.com/ktakashi/scheme-env/master/bin/install.sh | sh
```

After the installation you need to add the following to your shell
resource file:

```
PATH=~/.scheme-env/bin:$PATH
```

# How to use

The basic command id `scheme-env` if you want to run the default
implementation then use the following comment

```
$ scheme-env run
```

# Installing implementations

To install implementations, you can run the following command

```
$ scheme-env install implementation
```
Currently the followings are the supported implementation 

- Chibi Scheme (chibi-scheme)
- Sagittarius Scheme (sagittarius)

You can also specify the version by adding `@` and version number.
For example:

```
$ scheme-env install sagittarius@0.8.9
```

# Switch implementations

To swich default implementation, you can run the following command

```
$ scheme-env switch implementation
```
If this command isn't run, then `sagitarius` is set to default.
