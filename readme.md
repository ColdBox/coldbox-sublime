# A ColdBox Platform Bundle v2.0.0 for Sublime Text 2/3

Get the latest Sublime Text 2/3 from http://www.sublimetext.com/2.

## Target Platforms
- ColdBox 4.X.X
- TestBox 2.X.X

## Currently supported features

This bundle includes functionality not only for ColdBox MVC, but also for TestBox BDD/TDD, MockBox, WireBox, CacheBox and LogBox.

### Code Insight
Code completion for all major ColdBox + TestBox functions and scopes:

- `binder ➝` : "coldbox.system.ioc.config.Binder",
- `cachebox ➝` : "coldbox.system.cache.CacheFactory"
- `controller ➝` : "coldbox.system.web.Controller",
- `event ➝` : "coldbox.system.web.context.RequestContext",
- `flash ➝` : "coldbox.system.web.flash.AbstractFlashScope",
- `html ➝` : "coldbox.system.core.dynamic.HTMLHelper"
- `log ➝` : "coldbox.system.logging.Logger",
- `logbox ➝` : "coldbox.system.logging.LogBox",
- `wirebox ➝` : "coldbox.system.ioc.Injector",
- `$assert` : "testbox.system.Assertion"

### Code Skeleton Snippets

- `cachebox-config ➝` : Creates a new CacheBox.cfc configuration file
- `config ➝` : Creates a new ColdBox.cfc configuration file
- `bdd ➝` : Creates a TestBox BDD Bundle
- `box ➝` : Creates a `box.json` template
- `handler ➝` : Creates a ColdBox Event Handler
- `interceptor ➝` : Creates a ColdBox Interceptor
- `model ➝` : Creates a model object
- `routes ➝` : Creates a new routing file
- `point ➝` : Creates a new interception point method
- `unit ➝` : Creates a TestBox TDD xUnit Bundle

### Handler Code Snippets

- `action ➝` : Creates a handler action
- `around` : Creates an *aroundHandler()* implicit action
- `onerror ➝` : Creates an *onError()* implicit action 
- `onhttp ➝` : Creates an *onInvalidHTTPMethod()* implict action
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
- `o2m` : Creates a one-to-many property definition
- `m2o` : Creates a many-to-one property definition
- `m2m` : Creates a many-to-many property definition

### TestBox Snippets

- `assert` : An `assert()` method
- `afterAll ➝` : An `afterAll()` BDD life-cycle method
- `aftereach ➝` : An `afterEach()` BDD closure
- `afterTests ➝` : An `afterTests()` xUnit life-cycle method
- `aroundEach ➝` : An `aroundEach()` BDD closure
- `bdd ➝` : Creates a new BDD Test Bundle CFC
- `beforeAll ➝` : An `beforeAll()` BDD life-cycle method
- `beforeeach ➝` : A `beforeEach()` BDD closure
- `beforeTests ➝` : An `beforeTests()` xUnit life-cycle method
- `console ➝` : TestBox send some output to the console
- `debug ➝` : Writes up a non-duplicate `debug()` call
- `debugduplicate ➝` : Writes up a `debug()` call with duplicate
- `describe ➝` : A `describe` suite
- `describeFull ➝` : A `describe` suite with all arguments
- `expect ➝` : Starts an expectation DSL with a `toBe()` addition
- `expectAll ➝` : Starts a collection expectation DSL with a `toBe()` addition
- `expectFalse ➝` : Does a false expectation expression
- `expectTrue ➝` : Does a true expectation expression
- `expectToThrow ➝` : Starts an expectation that throws an exception
- `feature, featureFull ➝` : Starts a `feature()` block
- `given, givenFull ➝` : Starts a `given()` block
- `it ➝` : A test spec
- `itFull ➝` : A test spec with all arguments
- `setup ➝` : An `setup()` xUnit life-cycle method
- `story, storyFull ➝` : Starts a `story()` block
- `teardown ➝` : An `teardown()` xUnit life-cycle method
- `then, thenFull ➝` : Starts a `then()` block
- `unit ➝` : Creates a new xUnit Test Bundle CFC
- `when, whenFull ➝` : Starts a `when()` block 

### ColdBox Testing Snippets

- `handlerTest ➝` : Creates a ColdBox Event Handler test case
- `integration ➝` : Creates a top down integration BDD test case
- `interceptorTest ➝` : Creates an Interceptor test case
- `modelTest ➝` : Creates a model test case
- `testaction ➝` : Creates an integration spec case for an event action

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