# A ColdBox Platform Bundle for Sublime text 2

Get the latest Sublime Text 2 beta from http://www.sublimetext.com/2.

## Currently supported features

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
- `interceptor ➝` : Creates an Interceptor
- `model ➝` : Creates a model object
- `plugin ➝` : Creates a plugin
- `point ➝` : Creates a new interception point method

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

### Mac 

    $ cd ~/Library/Application\ Support/Sublime\ Text\ 2/Packages/
    $ git clone https://github.com/lmajano/cbox-coldbox-sublime.git coldbox
    
### Linux (Ubuntu like distros)

    $ cd ~/.config/sublime-text-2/Packages/
    $ git clone https://github.com/lmajano/cbox-coldbox-sublime.git coldbox

### Windows 7:

    Copy the directory to: "C:\Users\<username>\AppData\Roaming\Sublime Text 2\Packages"

### Windows XP:

    Copy the directory to: "C:\Documents and Settings\<username>\Application Data\Sublime Text 2\Packages"