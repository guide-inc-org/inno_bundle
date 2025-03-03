## 0.0.1

- Add a working bundler and example.

## 0.0.2

- Add a README.md to example and update main README.md.

## 0.0.3

- Fix `languages` attribute name in README.md example.

## 0.1.0

- Make `installer_icon` optional attribute.

## 0.1.1

- Update README.md.

## 0.2.0

- Update default icon, old one is not premissable to use for commercial use
  without license, so I created new one from **license free** resources.

- Clean cuportino icons from example as it is unused.

- Clean `lib\inno_bundle.dart` and `test\inno_bundle_test.dart`.

- When default icon is used, the new one is copied to `%TEMP%` folder on every
  installer build, I did not find an efficient way to update the old one.

## 0.3.0

- Replace `--skip-app` with `--app` and `--no-app` flags, default to `--app`.

- Add `--installer` and `--no-installer` flags, default to `--installer`.

- Add `--help` and `-h` with descriptive messages to each flag.

- Refactor `Config` to include cli arguments as well.

- Make `.iss script` generation happen under
  `build\windows\x64\installer\<BuildType>\<AppName>.iss`.

- Add `%UserProfile%\Local\Programs\Inno Setup 6` as a possible path to find
  Inno Setup installation.

- Update error message for option to install Inno Setup using `winget`
  when not detected on the machine.

## 0.3.1

- Update README.md for winget installation option of Inno Setup.

- Replace LinkedIn link in maintainer clause for generated `iss script` with
  GitHub link.

## 0.3.2

- Add documentation to codebase.

## 0.3.3

- Fix issue icon not persisting in the system temp directory when using
  default installer icon.

- Update iss script maintainer clause.

- Rename generated iss script to `inno-script.iss`.

## 0.4.0

- Add `--hf` and `--no-hf` flags to control printing of header and footer text.

- Add `--envs` to `build` command to print resolved config as environment
  variables and exit.

- Add `--help` to `id` command.

## 0.4.1

- Add guide to setup GitHub Workflows and automate installer build as GitHub releases.

## 0.4.2

- Update packages version and minimum dart and flutter version to latest.

## 0.5.0

- Update packages and lower back minimum dart and flutter versions.

- rework usage of app name and pubspec name props. See [#2](https://github.com/hahouari/inno_bundle/issues/2).
