# iOS-Project-Setup
checkpoints for new iOS project setup

### Git

- [ ] init gitIgnore, prefared to use [Github gitignore for swift](https://github.com/github/gitignore/blob/master/Swift.gitignore) , use [curl](https://gist.github.com/embassem/0da03355ddafade00e40aa65e8e482d5) to save file
- [ ] ignore Pods
- [ ] ignore Carthage Checkput , include Carthage *.frameworks (pro: faster build , con: increase project size ) [carthage](https://gist.github.com/embassem/b3eb762e62b23a50959285a5ad65ebc7)

### Package manager
- [ ] Cocoapods
- [ ] Carthage [prefared]

### Scripts
- [ ] Add Swiftgen for (Assets, Localizable, Fonts) 
- [ ] Add Swiftlint, customize Rulres, Prefared Restricted Rulre if starting Empty Project
- [ ] Add Bundler
- [ ] Add Makefile to wrap some Commands
- [ ] Add setup.sh script  to easly bootstrap the project
- [ ] Add bartycrouch to Localize XIB, Storyboards


### project Folder Structure

```
.
├── .bartycrouch.toml
├── .gitignore
├── .swiftlint.yml
├── AppStringsTemplete.stencil
├── Cartfile
├── Cartfile.resolved
├── CommitTemplet.txt
├── configuration.rb
├── Gemfile
├── Gemfile.lock
├── Makefile
├── Podfile
├── Podfile.lock
├── README.md
├── setup.sh
├── swiftgen.yml
│
├── App.xcodeproj
├── App.xcworkspace
│
├── APP
│   ├── AppClasses
│   │   ├── Bases
│   │   │   ├── Views
│   │   │   │   ├── BaseViewController.swift
│   │   │   │   └── BaseViewProtocol.swift
│   │   │   │
│   │   │   └── (Presenter / Model / ViewModel / Interactor)
│   │   │
│   │   ├── AppNavigationController.swift
│   │   └── AppTabBarViewController.swift
│   │
│   ├── Application
│   │   ├── AppDelegate.swift
│   │   ├── AppManager.swift
│   │   └── SceneDelegate.swift
│   │
│   ├── Configeration
│   │   ├── Environment.swift
│   │   ├── Base.xcconfig
│   │   ├── Debug.xcconfig
│   │   └── Release.xcconfig
│   │
│   ├── Extensions
│   │   ├── Result.swift
│   │   ├── UINavigationBar.swift
│   │   ├── UINavigationController.swift
│   │   ├── UINavigationItem.swift
│   │   └── UIWindow+Transition.swift
│   │     
│   │ 
│   ├── Features (OR Scenes)
│   │   ├── Foo
│   │   │   └── Replaceme.swift
│   │   ├── Boo
│   │       └── Replaceme.swift
│   │
│   ├── LaunchScreen
│   │    ├── Splash
│   │    │   ├── SplashViewController.xib
│   │    │   └── SplashViewController
│   │    └── LaunchScreen.storyboard
│   │
│   ├── Resources
│   │   ├── Assets
│   │   │   ├── Assets.swift
│   │   │   └── Assets.xcassets
│   │   │
│   │   ├── Fonts
│   │   │   ├── Fonts.swift
│   │   │   └── ScaledFont.swift
│   │   │
│   │   ├── Localization
│   │   │   ├── Localizable.strings
│   │   │   ├── Localized+Runtime.swift
│   │   │   └── Localized.swift
│   │   │
│   │   └── OTHERS
│   │ 
│   ├── Services
│   │   ├── Container.swift
│   │ 
│   └── SupportingFiles
│           └── Info.plist
├── Networking
│
├── FrameworkA
│
├── FrameworkB
│
└─────────────────────────
```

### select your App Project
form inspector set Project Format to Latest Xcode Support
