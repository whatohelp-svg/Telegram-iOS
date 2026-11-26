# RiseGram Apple native core

Experimental source port shared by iOS and macOS. Uses the Android client's DC2 TCP endpoint and pinned server public RSA key. Cached or discovered public routes are not selected by the address-set lookup. Public backup address discovery is disabled. This is not a release: separate app identifiers, signing, push configuration, Rust transport and proxy audit, native build and on-device authentication, session persistence, media and economy tests are required. Do not reuse Telegram application containers or publish an untested IPA.

## CI builds

The experimental arm64 build runs on pushes to `risegram/native-port`. Configure `RISEGRAM_IOS_BUILD_CONFIG` as an Actions secret before building; fake signing is for experimental packaging only and does not establish installability on a physical iPhone.
