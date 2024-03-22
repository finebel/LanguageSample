# LanguageSample

This is a demo project showcasing an issue when using `xcodebuild -exportLocalization` due to the usage of R.swift.

```
xcodebuild -exportLocalizations \
-project LanguageSample.xcodeproj \
-localizationPath "<export path>" \
-exportLanguage en
```
The above command will produce a `cannot find 'R' in scope` build error for the usage of `R.string.localizable.sample_test()` in `ViewController.swift`.
