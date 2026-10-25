# Local compatibility backport

Source: https://github.com/jac3km4/red4ext-rs at d419d98d8b81a19a62585d11759fabdeabeb0957 (MIT; see LICENSE).
SDK submodule: WopsS/RED4ext.SDK at 5246e659d783e5834cc08a90e56c8932c9ed3449.

Only src/types/callback.rs, src/types/rtti.rs and src/types/array/mod.rs differ from that dependency revision. They adapt the fixed callback buffer, RTTI bindings and DynArray storage to Cyberpunk 2077 2.50. Registration/export semantics are retained because Audioware uses script-defined parameter classes resolved later by REDscript.

Initialize dependencies with git submodule update --init --recursive before building. This is a startup compatibility backport, not a complete gameplay compatibility claim. Audioware author PR #104 includes additional game-layout changes not included here.
