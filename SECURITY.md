# Security Policy

## Supported Versions

We actively support the latest stable release of Anomalous Field Recorder and security-critical branches under long-term support (LTS).

| Version | Supported |
|---------|-----------|
| main    | ✅        |
| LTS-*   | ✅        |
| others  | ❌       |

Security fixes will be backported to maintained branches on a best-effort basis.

## Reporting a Vulnerability

If you discover a security vulnerability, please follow these steps:

1. **Do not create a public issue.**
2. Email the security team at [security@anomalousfield.io](mailto:security@anomalousfield.io) with the subject line `Security Vulnerability Report`.
3. Include the following details:
   - Description of the vulnerability
   - Affected components (files, endpoints, configurations)
   - Steps to reproduce, including scripts or payloads when applicable
   - Impact assessment and potential mitigations

You can optionally encrypt your report using our PGP key:

```
-----BEGIN PGP PUBLIC KEY BLOCK-----
Version: GnuPG v2

mQENBGQpN+IBCADRqCynux0LFskwg1Tl2iYyAPrFoP9Y5X1gP1EPnUArct7sVCU8
fViVgHmfZg/3gso5k8zDEADyfbPrK6k3NcZY35ZPgY9ruI3+Wk9ZweFcPz9rJkMk
u1fp78G1BrYF/pcP/PFivO2AyqQMBws9K0T2Ns8W5ml2Wj6a6GTYQxcZbL3OwXLP
XSSEn23jCu3PZeRVvSBvfdkPfnkx62RLGtWJJNNTkfRuSlaVJB/8Sj/4bQ3dxJgw
hBPgrr5Oy1ZdCX6bKtk+OXS1oXcXvuJ0CKztnT0A03D3LQyJR6SOYcsoh+7qfZ3x
U3r4E9f7eVwT1EfsGX+yxv9xm4zrrbK7jqe1ABEBAAG0IUFub21hbG91cyBGaWVs
ZCBSZWNvcmRlciBTZWN1cml0eSBUZWFtiQFUBBMBCgA+AhsDBQsJCAcCBhUICQoL
AgQWAgMBAh4BAheAFiEELcB3TbaZm0csPM8DZ7CLpWdectAFAmQpN+ICGy8FCQlm
AYAACgkQZ7CLpWdectChEwf+IbNdOu8Mz7ikxuOb+p3i1nZAy1dSN3HChbPH3lSQ
YIorxojCVgOeo1qBdRUrALs14mIuE6YZtuCeiO6YPtUWTy5mwUpMvhkWd6n5y7Vz
c7CYAt//S6GDu0Pd9ft7TgebuM8dyPmp6lHQ46r8BS3GJ4dY4cIdLyIpExgnKdmA
MLkuq3CLjuQnT6VE5kFxPW28+4TRlAz96khQwxv1DvU1X5f8h7sBKQAaO5rhFiHK
LcaIK4+kwhoDjyJdiI1sqi2kt5ftA3Ze8ZKe35epqOkwb2cYZLx1XvSKQhvTsbkB
Ijppf+UPznBDixr9fB0cJQwCBze916+S4Cbmt8C3x2i/kR9LMuRpGJtfuQENBGQp
N+IBCADg7O3PeY0nS7cnO4OIrH2iLQbA0jdrnvmGwTlsK25c9CrcXoV0XeFuNXOz
mg6g6OOaM7qd1OZjg70VPa3ZPrNYWqOlpjYkGttVmcEYXk7Gbv7nLZoOt2xqJAVf
PjN3iXFFzu7IE0XsgLbJMe2SxhNb2LtYKfQaiCG7kQ7BIJTIUTmZjDYQJrXLr9+g
lgVKtk1F9YmqlJAszTu8EImMB0Pa0k5Ht7/ICjXHm0ceT+e1a9cfSZQ/0AA0dgyR
xm6Y2BKbnN7ghMCIfQyznRy7cMX98xPiQEcY+u1eFzp5pyigVtvv3RSUXFZXvl42
nJqNRn+O8G8hLzAMiPp8V8G9CZIeGKiXABEBAAGJAR8EGAEKAAkFAmQpN+ICGy4C
SQkQZ7CLpWdectCBdCAEGQEKAB0WIQQtwHdNtpmbRyw8zwNnsIulZ15y0AUCZCk3
4gAKCRBnsIulZ15y0As3B/99/pZCqgFKbDn3h77/gKX2UDnM2hyTzrWHpDo9CV3Q
0yKyGv0pQ/9p3XP2/1fUZRrQ2XtA7M3EkyG3vjpz9aALMbBBV3NHGYbtJc0aoX0v
StU6cu+VhdfjqdwJYMApjbx3ko5UhxFJKT7N2yZBcvGmqFFJ6SyUu8N9AgJQrq3+
CWMokgJIa5G7t+n9pgmMtd19mhHy8dYt3v6p8vqek0ujgYK/JNp6lpNi2PvQgpiO
jxRtRvQSyAJwSTmXTO2Hd7VCRgNgV7CMz1Pg3wuIBtG9KKZRcmTSSl4XXGmpQxEX
LBNfXVSYGttQGGhIZ1VUtbbO4brvYcCB6VVc6Hqvgg==
=slJ3
-----END PGP PUBLIC KEY BLOCK-----
```

We aim to acknowledge receipt within 3 business days and provide an estimated timeline for remediation. Once the vulnerability is resolved, we will coordinate disclosure with you.

## Security Updates

Security advisories will be published through GitHub Security Advisories and mirrored in `docs/security/advisories/`.

## Responsible Disclosure

Please keep vulnerabilities confidential until a fix has been released. Do not test vulnerabilities against production infrastructure without explicit permission.

Thank you for helping us keep Anomalous Field Recorder secure.

