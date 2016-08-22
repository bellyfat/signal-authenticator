# Contributing

Looking to contribute? Great!
Remember to rebase to my master branch before submitting any pull requests.
Here are some low-hanging fruit:

- Test on a variety of different machines, architectures, etc.
- Stress test.
- Find and fix typos or otherwise improve clarity in the README.
- Improve the signal-auth-setup shell script for clarity and robustness.
- Write a man page.
- Create unit tests.
- Contribute to OpenSSH to resolve
[bug #2246](https://bugzilla.mindrot.org/show_bug.cgi?id=2246)
so that we can finally have (Public key AND Signal) OR (Password AND Signal)
authentication.
- Contribute to signal-cli.
- Begin process of packaging for your distro.

## Hacking

The `pam_syslog` function is useful for testing,

```
pam_syslog(pamh, LOG_INFO, "%s %d", "printf like formatting", 7);
```

and results appear in your syslog.
