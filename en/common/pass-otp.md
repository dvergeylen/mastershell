---
layout: default
title: "pass otp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pass-otp">
  <a href="/en/common/pass-otp.html">pass otp</a> <a href="#pass-otp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A pass extension for managing one-time-password (OTP) tokens.
> More information: <https://github.com/tadfisher/pass-otp#readme>.

#### Prompt for an otpauth URI token and create a new pass file:
```shell
pass otp insert {{path/to/pass}}
```
#### Prompt for an otpauth URI token and append to an existing pass file:
```shell
pass otp append {{path/to/pass}}
```
#### Print a 2FA code using the OTP token in a pass file:
```shell
pass otp {{path/to/pass}}
```
#### Copy and don't print a 2FA code using the OTP token in a pass file:
```shell
pass otp --clip {{path/to/pass}}
```
#### Display a QR code using the OTP token stored in a pass file:
```shell
pass otp uri --qrcode {{path/to/pass}}
```
#### Prompt for an OTP secret value specifying issuer and account (at least one must be specified) and append to existing pass file:
```shell
pass otp append --secret --issuer {{issuer_name}} --account {{account_name}} {{path/to/pass}}
```
{% endraw %}