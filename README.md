title: Password 💀
author:
  name: I'm Adrien, frontend developer
  email: a.gibrat@oodrive.com
theme: ./theme
controls: false
output: index.html

--

# Password 💀

--

## Password sucks

<center>Since 2018, Microsoft advocate<br>[The beginning of "The end of passwords"](https://www.microsoft.com/en-us/security/technology/identity-access-management/passwordless)</center>

<span class="fragment" data-icon="🔓">not secure <small>[haveibeenpwned](https://haveibeenpwned.com/unifiedsearch/s.deremur%40oodrive.fr) 408 leaked
dataset = 8 506 873 299 accounts</small></span><br>
<span class="fragment" data-icon="😱">not user friendly <small>[password = complexity](https://uxplanet.org/why-complex-passwords-are-bad-design-and-5-ways-to-do-better-affcc4516406) your mom doesn't use a password manager</small></span><br>

-- screen full

[![Password strength misconception](img/password_strength.png)](https://xkcd.com/9368a8cde/ "xkcd, the universal source of truth")

--

### Password policies 💩

<center>various best practices [ANSSI](https://www.ssi.gouv.fr/guide/mot-de-passe/ "Agence Nationale de la Sécurité des Systèmes d'Information") ⚡ [NIST](https://pages.nist.gov/800-63-3/sp800-63b.html#sec5 "National Institute of Standards and Technology")</center>

<span class="fragment check" data-icon="✓">never reuse password</span><br>
<span class="fragment check" data-icon="✓">use passphrase</span><br>
<span class="fragment check" data-icon="✓">check against lists (contextual, dictionary, common, leaked…)</span><br>
<span class="fragment check" data-icon="✓">SMS is [not secure](https://www.bankinfosecurity.com/heres-account-authentication-shouldnt-use-sms-a-11708) OTP (PSD2: banking deprecated SMS)</span><br>
<span class="fragment check" data-icon="💥">force special characters <small>leet `Oodrive$1`</small></span><br>
<span class="fragment check" data-icon="💥">force periodic password changes <small>#… `Oodrive9`</small></span><br>

-- screen large

### Forget password 😡

![User experience when forgot password](img/forget_password.gif)

-- screen large

### Expired password 🤬 

![User experience when password expires](img/expired_password.gif)

-- screen

## FIDO <small class="fragment">[alliance](https://fidoalliance.org/members/)</small> 👀

<center class="fragment">Fast ID online <small>[Solving the World's Password Problem](https://fidoalliance.org/what-is-fido/)</small></center>

[![Fast ID online](img/fido.gif)](https://fidoalliance.org/)

--

### Specifications 🤖

- FIDO U2F <small>Universal *Second Factor authentication*</small><br><small class="fragment">using asymetric cryptography with USB security key (+ NFC / BLE)</small>
- FIDO UAF <small>Universal Authentication Framework</small><br><small class="fragment">*Passwordless Authentication* with biometrics & external security device</small>
- FIDO2 [W3C WebAuthn](https://www.w3.org/TR/webauthn-1/) <small>(March 2019) API for accessing Public Key</small><br><small class="fragment">Secure passwordless & multi-factor authentication for the web</small>

-- screen

### Client to Authenticator Protocol 🤓

[![WebAuthn + CTAP Flow](img/fido2_flow.jpg)](https://fidoalliance.org/fido2/)

<center  class="fragment" style="background-repeat:no-repeat;background-image:url(img/phone.png); background-position: 4em top"> = cryptographic & biometric proof, NOT SMS<sup><small>™</small></sup><br><br></center>


<center>[CTAP 2](https://en.wikipedia.org/wiki/Client_to_Authenticator_Protocol) = WebAuthn authenticator specification
<br>(CTAP 1 = U2F only)</center>

-- screen

### FIDO 2 support 💪

[![WebAuthn support](img/fido2_support.jpg)](https://fidoalliance.org/fido2/fido2-web-authentication-webauthn/)

<center>[Windows 10](https://fidoalliance.org/microsoft-achieves-fido2-certification-for-windows-hello/), [Android 7+](https://fidoalliance.org/android-now-fido2-certified-accelerating-global-migration-beyond-passwords/)(1B+ devices)<br>& all evergreen browsers, including [Safari](https://webkit.org/blog/8517/release-notes-for-safari-technology-preview-71/)</center>

-- screen

## Demo 👩‍💻


[![WebAuthn demo](img/webauthn_io.png)](https://webauthn.io)

<center>https://webauthn.io</center>

-- screen

### Simple worklow 🤗

<div style="float:left;width: 50%">
**Registration**
[![WebAuthn register worklow](img/webauthn_register.jpg)](https://webauthn.guide/)
</div>

<div style="float:left">
**Login**
[![WebAuthn login worklow](img/webauthn_login.jpg)](https://fidoalliance.org/key-differentiators/)
</div>

--

### Password is dead, long live the password 👑

> [300 billion passwords by 2020 <br>$6 trillion annual damage by 2021](https://thycotic.com/wp-content/uploads/2013/03/Cybersecurity-Ventures-Thycotic_Password-Protection.pdf)

> [Do FIDO2 passwordless & WebAuthn](https://developer.mozilla.org/en-US/docs/Web/API/Web_Authentication_API) today!
> <br>FIDO is already a [requirement for banking](https://fidoalliance.org/fido-standards-meet-psd2-sca-requirements/) <br>and will be one soon for other regulated industries.
