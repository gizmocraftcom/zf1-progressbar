# Changelog
## 2.0.0
Fork of `diablomedia/zendframework1-progressbar`, published as `gizmocraft/zendframework1-progressbar`.
### Breaking changes
- Requires PHP `>=8.5`. Tested on PHP 8.5 and 8.6.
- Package renamed from `diablomedia/zendframework1-progressbar` to `gizmocraft/zendframework1-progressbar`. It now requires `gizmocraft/zendframework1-exception` `^2.0.0`, `gizmocraft/zendframework1-config` `^3.0.0`, `gizmocraft/zendframework1-json` `^2.0.0`, `gizmocraft/zendframework1-text` `^2.0.0` and `gizmocraft/zendframework1-session` `^3.0.0`.
### Other changes
- No public signature changes.
- `Zend_ProgressBar_Adapter_Console::setWidth()` uses `is_int()` instead of `is_integer()`, which PHP 8.6 deprecates.
- Dev dependencies upgraded (PHPUnit 13, PHPStan 2.3, php-cs-fixer 3.95, GrumPHP 2.27). Dropped `composer-require-checker`, which has no release for PHP 8.6.
- Tests migrated to PHPUnit 13 attributes.
- CI runs PHP 8.5 and 8.6.
