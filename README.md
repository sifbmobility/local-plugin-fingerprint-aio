# Customized

local_plugins\cordova-plugin-fingerprint-aio\1.7.0\cordova-plugin-fingerprint-aio\plugin.xml

- Added custom message return to cordova when passcode is locked (IOS).

- biometric dependecy upgrade - build.gradle
  upgrade to androidx.biometric:biometric:1.1.0

- added import at line 15
  import androidx.biometric.BiometricManager;

- added at line 95 - method createPromptInfo  
  .setAllowedAuthenticators(BiometricManager.Authenticators.BIOMETRIC_STRONG)

===
file changed(apps/showroom-mb/local_plugins/cordova-plugin-fingerprint-aio/5.0.1/cordova-plugin-fingerprint-aio/package.json)

Remove "cordova-paramedic": "git+https://github.com/apache/cordova-paramedic", from devdependencies to settle NPM audit vulnerabilities problem

# Installation

If your platforms having the existing plugin, remove it first. Make sure platforms & plugins do not have the plugins.

- Remove plugin
  cordova plugin rm cordova-plugin-fingerprint-aio

- Add plugin
  cordova plugin add ./apps/showroom-mb/local_plugins/cordova-plugin-fingerprint-aio/5.0.1/cordova-plugin-fingerprint-aio
