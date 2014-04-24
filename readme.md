# A ColdBox Platform Bundle v1.7 for Sublime text 2

Get the latest Sublime Text 2 from http://www.sublimetext.com/2.

## Currently supported features

### Code Insight
Code completion for all major ColdBox functions and scopes:

- `controller ➝` : "coldbox.system.web.Controller",
- `event ➝` : "coldbox.system.web.context.RequestContext",
- `flash ➝` : "coldbox.system.web.flash.AbstractFlashScope",
- `log ➝` : "coldbox.system.logging.Logger",
- `logbox ➝` : "coldbox.system.logging.LogBox",
- `binder ➝` : "coldbox.system.ioc.config.Binder",
- `wirebox ➝` : "coldbox.system.ioc.Injector",
- `cachebox ➝` : "coldbox.system.cache.CacheFactory"

### Handler Code Snippets

- `action ➝` : Creates a handler action
- `onerror ➝` : Creates an *onError()* implicit action 
- `onma ➝` : Creates an *onMissingAction()* implicit action 
- `postaction ➝` : Creates a *postXXX()* implicit action 
- `post ➝` : Creates a *postHandler()* implicit action 
- `preaction ➝` : Creates a *preXXX()* implicit action 
- `pre ➝` : Creates a *preHandler()* implicit action 

### ORM Code Snippets

- `active ➝` : Creates a ColdBox Active Entity
- `entity ➝` : Creates an ORM Entity
- `ormservice ➝` : Creates a Base ORM service
- `virtualservice ➝` : Creates a virtual entity service

### Code Skeleton Snippets

- `handler ➝` : Creates a ColdBox Event Handler
- `interceptor ➝` : Creates a ColdBox Interceptor
- `point ➝` : Creates a new interception point method
- `model ➝` : Creates a model object
- `plugin ➝` : Creates a ColdBox plugin
- `config ➝` : Creates a new ColdBox.cfc configuration file
- `cachebox-config ➝` : Creates a new CacheBox.cfc configuration file
- `routes ➝` : Creates a new routing file

### TestBox Snippets

- `bdd ➝` : Creates a new BDD Test Bundle CFC
- `unit ➝` : Creates a new xUnit Test Bundle CFC
- `describe ➝` : A `describe` suite
- `describeFull ➝` : A `describe` suite with all arguments
- `it ➝` : A test spec
- `itFull ➝` : A test spec with all arguments
- `expect ➝` : Starts an expectation DSL with a `toBe()` addition
- `expectFalse ➝` : Does a false expectation expression
- `expectTrue ➝` : Does a true expectation expression
- `expectToThrow ➝` : Starts an expectation that throws an exception
- `afterAll ➝` : An `afterAll()` BDD life-cycle method
- `beforeAll ➝` : An `beforeAll()` BDD life-cycle method
- `aftereach ➝` : An `afterEach()` BDD closure
- `beforeeach ➝` : A `beforeEach()` BDD closure
- `afterTests ➝` : An `afterTests()` xUnit life-cycle method
- `beforeTests ➝` : An `beforeTests()` xUnit life-cycle method
- `teardown ➝` : An `teardown()` xUnit life-cycle method
- `setup ➝` : An `setup()` xUnit life-cycle method
- `debug ➝` : Writes up a non-duplicate `debug()` call
- `debugduplicate ➝` : Writes up a `debug()` call with duplicate
- `console ➝` : TestBox send some output to the console

### Unit-Integration Testing Snippets

- `handlerTest ➝` : Creates a ColdBox Event Handler test case
- `integrationTest ➝` : Creates a top down integration test case
- `integrationTestCase ➝` : Creates a test case for an event action
- `interceptorTest ➝` : Creates an Interceptor test case
- `modelTest ➝` : Creates a model test case
- `pluginTest ➝` : Creates a plugin test case

### WireBox Code Snippets

- `aspect ➝` : Creates a WireBox AOP Aspect object
- `binder ➝` : Creates a basic WireBox configuration binder
- `inject ➝` : WireBox property injection
- `provider ➝` : Creates a WireBox provider method
- `setter ➝` : Creates a WireBox setter injection

## Installation instructions : 

### With Package Control ###

If you have the [Package Control](http://wbond.net/sublime_packages/package_control) package installed, you can install *ColdBox Platform Bundle* from inside Sublime Text itself. Open the Command Palette and select "Package Control: Install Package", then search for *ColdBox*.

### Without Package Control ###

#### Mac 

    $ cd ~/Library/Application\ Support/Sublime\ Text\ 2/Packages/
    $ git clone https://github.com/lmajano/cbox-coldbox-sublime.git coldbox
    
#### Linux (Ubuntu like distros)

    $ cd ~/.config/sublime-text-2/Packages/
    $ git clone https://github.com/lmajano/cbox-coldbox-sublime.git coldbox

#### Windows 7:

    Copy the directory to: "C:\Users\<username>\AppData\Roaming\Sublime Text 2\Packages"

#### Windows XP:

    Copy the directory to: "C:\Documents and Settings\<username>\Application Data\Sublime Text 2\Packages"

## References:

- Sublimetext 2 API - http://www.sublimetext.com/docs/2/api_reference.html
- How to create a plugin: http://net.tutsplus.com/tutorials/python-tutorials/how-to-create-a-sublime-text-2-plugin/
- Unoffical (but very good) docs - http://sublimetext.info/docs/en/
- ColdFusion Sublime Text bundle - https://github.com/SublimeText/ColdFusion
- MXUnit Sublime Text bundle - https://github.com/mxunit/sublime-text-2-mxunit

## Changelog
### v1.7
- TestBox additions
- Testing additions

### v1.5
- Handler snippet fixes
- Model skeleton fix
- New `config` skeleton for the Configuration File
- New `cachebox-config` skeleton for a CacheBox Configuration File
- New `routes` skeleton for a routes.cfm template
- Completions for ALL ColdBox related functions and major scopes

### v1.0 Initial Release