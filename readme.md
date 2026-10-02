# ColdBox Platform Bundle for Sublime Text

Code completions and snippets for the [ColdBox Platform](https://coldbox.org) and [TestBox](https://testbox.ortusbooks.com) on **Sublime Text 4**.

## Supported Versions

| Library | Supported Versions | Notes |
|---------|--------------------|-------|
| ColdBox | **8.0.0 and beyond** | Includes WireBox, CacheBox and LogBox |
| TestBox | **7.0.0 and beyond** | Includes the 7.1 expectation and assertion additions |
| Sublime Text | **4** | |

| Language / Engine | Status |
|-------------------|--------|
| BoxLang | Preferred |
| Lucee | Supported |
| Adobe ColdFusion | Supported |

> Using ColdBox 7 or TestBox 6? Use the `v3.2.x` tags of this package.

Completions and snippets that arrived in a specific release are labeled with the version in the completion popup, for example `(ColdBox:Router - 8.2+)` or `(TestBox:Expectation - 7.1+)`.

## Installation

### Package Control (recommended)

1. Open the Command Palette (`Cmd/Ctrl + Shift + P`)
2. Select **Package Control: Install Package**
3. Search for **ColdBox** and install it

### Manual

Clone the repository into your Sublime Text `Packages` directory (use **Preferences > Browse Packages...** to find it).

```bash
# macOS
cd ~/Library/Application\ Support/Sublime\ Text/Packages/
# Linux
cd ~/.config/sublime-text/Packages/
# Windows (PowerShell)
cd "$env:APPDATA\Sublime Text\Packages"

git clone https://github.com/ColdBox/coldbox-sublime.git coldbox
```

## Features

### Code Insight

Completions for the major ColdBox, WireBox, CacheBox, LogBox and TestBox objects. Type the scope name and a dot to see its methods.

| Scope | Class |
|-------|-------|
| `event` | `coldbox.system.web.context.RequestContext` |
| `controller` | `coldbox.system.web.Controller` |
| `flash` | `coldbox.system.web.flash.AbstractFlashScope` |
| `html` | `coldbox.system.modules.HTMLHelper.models.HTMLHelper` |
| `binder` | `coldbox.system.ioc.config.Binder` |
| `wirebox` | `coldbox.system.ioc.Injector` |
| `cachebox` | `coldbox.system.cache.CacheFactory` |
| `logbox` | `coldbox.system.logging.LogBox` |
| `log` | `coldbox.system.logging.Logger` |
| `assert` | `testbox.system.Assertion` |

Also included:

- **Handlers, RestHandlers, Interceptors and the framework super type** methods
- **Router DSL** (bare functions inside `config/Router`): `route()`, `resources()`, `apiResources()`, `group()`, the verb helpers (`get()`, `post()`, `put()`, `patch()`, `delete()`), `.to()`, `.toHandler()`, `.toAction()`, `.toView()`, `.toResponse()`, `.toRedirect()`, `.as()`, `.withCondition()`, `.withSSL()`, `.withVerbs()`, `.withNamespace()`, `.withDomain()`, `.constraints()`, `.end()` and more
- **ColdBox 8.1+/8.2+ additions**: `.middleware()`, `middlewareGroup()`, `.withoutMiddleware()`, `.withCache()`, `.toSSE()`, `.toAi()`, `.toMCP()`, `.toAiGateway()`, plus `event.sse()`, `event.etag()`, `event.lastModified()` and `event.cacheControl()`
- **TestBox expectations**: every `expect()` matcher, including the 7.1 additions: `toBeTruthy`, `toBeFalsy`, `toHaveSize`, `toThrowMatching`, `toIncludeAll/Any/None`, Set matchers, Range matchers and data path matchers (`toHavePath`, `toHavePathValue`, ...)
- **TestBox collection and grouped checks**: `expectAll()`, `expectAny()`, `expectSome()`, `expectNone()`, `withContext()`, `assertAll()`, `assert.all()`
- **TestBox `dryRun()`** to discover specs without executing them

### Snippets

Type the trigger and press `Tab`.

#### Skeletons

| Trigger | Creates |
|---------|---------|
| `config` | `ColdBox` configuration file |
| `router` | Router file |
| `handler` | Event handler |
| `resthandler` | REST handler |
| `resourcehandler` | Resource handler |
| `apiResourceHandler` | API resource handler |
| `model` | Model object |
| `interceptor` | Interceptor |
| `point` | Interception point method |
| `cachebox-config` | `CacheBox` configuration file |
| `box` | `box.json` descriptor |

#### Language

| Trigger | BoxLang | CFML |
|---------|---------|------|
| `class` | Class | |
| `cfc` | | Script component |
| `function` | Function | Script function |
| `prop` | Property | Script property |
| `inject` | WireBox property injection | WireBox property injection |

#### Handlers

| Trigger | Creates |
|---------|---------|
| `action` | Handler action |
| `pre` / `post` | `preHandler()` / `postHandler()` |
| `preaction` / `postaction` | `preXXX()` / `postXXX()` |
| `around` | `aroundHandler()` |
| `onerror` | `onError()` |
| `onhttp` | `onInvalidHTTPMethod()` |
| `onma` | `onMissingAction()` |

#### WireBox

| Trigger | Creates |
|---------|---------|
| `binder` | WireBox configuration binder |
| `inject` | Property injection |
| `setter` | Setter injection |
| `provider` | Provider method |
| `aspect` | AOP aspect |

#### ORM

| Trigger | Creates |
|---------|---------|
| `entity` | ORM entity |
| `active` | Active entity |
| `ormservice` | Base ORM service |
| `virtualservice` | Virtual entity service |
| `o2m` / `m2o` / `m2m` | Relationship properties |

#### TestBox

| Trigger | Creates |
|---------|---------|
| `bdd` / `unit` | BDD / xUnit test bundle |
| `describe`, `it`, `feature`, `story`, `given`, `when`, `then` | BDD blocks (add `Full` for all arguments) |
| `beforeall`, `afterall`, `before`, `after`, `around` | BDD life-cycle closures |
| `beforetests`, `aftertests`, `setup`, `teardown` | xUnit life-cycle methods |
| `expect`, `expectTrue`, `expectFalse`, `expectToThrow` | Expectations |
| `expectall`, `expectany` `7.1+`, `expectsome` `7.1+`, `expectnone` `7.1+` | Collection expectations |
| `withcontext` `7.1+` | Expectation with failure context |
| `expectpath` `7.1+` | Data path expectation |
| `assert`, `assertall` `7.1+` | Assertions |
| `dryrun` `7.0+` | Discover specs without running them |
| `debug`, `debugduplicate`, `console` | Debug output |

#### ColdBox Testing

| Trigger | Creates |
|---------|---------|
| `integrationTest` | Integration BDD test |
| `testaction` | Integration spec for an event action |
| `interceptorTest` | Interceptor test |
| `modelTest` | Model test |

## Contributing

Issues and pull requests are welcome at <https://github.com/ColdBox/coldbox-sublime>. See the [changelog](changelog.md) for release history.

## References

- [ColdBox Documentation](https://coldbox.ortusbooks.com)
- [TestBox Documentation](https://testbox.ortusbooks.com)
- [Sublime Text API](https://www.sublimetext.com/docs/api_reference.html)
- [ColdFusion Sublime Text bundle](https://github.com/SublimeText/ColdFusion)
