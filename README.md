check-s2s-ciphers
=================

This is a quick'n'dirty script to check the TLS [cipher suites][1] offered by
an [XMPP][2] server when [another server connects][3].  The script is called
like this:

    check-s2s-ciphers xmpp.example.net

Where `xmpp.example.net` is the actual host name of the XMPP server (i.e., the
`check-s2s-ciphers` script won't perform SRV record lookups).

Only those ciphers supported by the local [OpenSSL][4] version can be checked.

[1]: https://www.openssl.org/docs/apps/ciphers.html
[2]: http://xmpp.org/
[3]: https://tools.ietf.org/html/rfc6120#section-9.2.1
[4]: https://www.openssl.org/
