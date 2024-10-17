# Google Authenticator

Ported from http://code.google.com/p/google-authenticator/

You can use the Google Authenticator app from here
http://www.google.com/support/accounts/bin/answer.py?hl=en&answer=1066447
to generate One Time Passwords/Tokens and check them with this little
PHP app (Of course, you can also create them with this).

[![Latest Stable Version](https://poser.pugx.org/clsystem/google-authenticator/v/stable)](https://packagist.org/packages/clsystem/google-authenticator)
[![Latest Unstable Version](https://poser.pugx.org/clsystem/google-authenticator/v/unstable)](https://packagist.org/packages/clsystem/google-authenticator)
[![License](https://poser.pugx.org/clsystem/google-authenticator/license)](https://packagist.org/packages/clsystem/google-authenticator)

[![Total Downloads](https://poser.pugx.org/clsystem/google-authenticator/downloads)](https://packagist.org/packages/clsystem/google-authenticator)
[![Monthly Downloads](https://poser.pugx.org/clsystem/google-authenticator/d/monthly)](https://packagist.org/packages/clsystem/google-authenticator)
[![Daily Downloads](https://poser.pugx.org/clsystem/google-authenticator/d/daily)](https://packagist.org/packages/clsystem/google-authenticator)

Branch | Github Actions | Coverage |
------ | -------------- | -------- |
2.x    | [![Test][test_stable_badge]][test_stable_link]     | [![Coverage Status][coverage_stable_badge]][coverage_stable_link]     |

## Installation using Composer

```bash
composer require clsystem/google-authenticator
```

## Usage

See example.php for how to use it.

There's a little web app showing how it works in web/, please make users.dat
writeable for the webserver, doesn't really work otherwise (it can't save the
secret). Try to login with chregu/foobar.

What's missing in the example:

 * Prevent replay attacks. One token should only be used once
 * Show QR Code only when providing password again (or not at all)
 * Regenerate secret

## Support


This package is available under the [MIT license](LICENSE).

[test_stable_badge]: https://github.com/clsystem/GoogleAuthenticator/workflows/Test/badge.svg?branch=2.x
[test_stable_link]: https://github.com/clsystem/GoogleAuthenticator/actions?query=workflow:test+branch:2.x

[coverage_stable_badge]: https://codecov.io/gh/clsystem/GoogleAuthenticator/branch/2.x/graph/badge.svg
[coverage_stable_link]: https://codecov.io/gh/clsystem/GoogleAuthenticator/branch/2.x
