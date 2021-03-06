# Phone Number Preference

Ever wanted to add a phone number in your android shared preferences. This library will help with that.  Simply add straight into your preferences.xml and you're away.

<img src="https://user-images.githubusercontent.com/16980993/30968294-bfdefe6a-a456-11e7-9187-b76d30dc2519.png" width="255">

## Usage

Add this to your module dependencies:
```groovy
    compile 'com.nfx.android:phone-number-preference:latest-version'
````

Now just add the preference to to your preference xml file like any other preference
```xml
  <com.nfx.android.phonenumberpreference.PhoneNumberPreference
      android:key="your_pref_key"
      android:title="Preference Key"
      android:summary="A summary of the preference"

      app:rbp_measurementUnit="unit text"
      app:rbp_tickStart="1"
      app:rbp_tickEnd="100"
      app:rbp_tickInterval="1"
      app:rbp_view_defaultLowValue="40"
      app:rbp_view_defaultHighValue="60"/>
````

If you have to support API-v7+, this lib provides also PhoneNumberPreferenceCompat that works with preference-v7.
```xml
  <com.nfx.android.phonenumberpreference.PhoneNumberPreferenceCompat
      android:key="your_pref_key"
      android:title="Preference Key"
      android:summary="A summary of the preference"

      app:pnp_default_phone_number="123456789"
      app:pnp_view_enabled="true"/>
````

## Versioning

[SemVer](http://semver.org/) is used for versioning. For the versions available, see the [tags on this repository](https://github.com/nfxdevelopment/phone-number-preferences/tags).

## Authors

* **Nicholas Winder** - *Preference adaptation work* - [nick winder](https://github.com/nickwinder)

## Licence
Licenced under *Apache2 licence*, so you can do whatever you want with it.
Please push back changes to help the library mature.

## Acknowledgments

* Thanks to [oli107](https://github.com/oli107) for the orignal range bar library.
