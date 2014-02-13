node-module-demo
================

Illustration of how Node modules can depend on different versions of the same module without conflicting.

Node's module resolution will look for dependencies in the nearest `node_modules` folder.

Unlike Ruby, `require`'s do not *usually* change any global state. You do not `require('express')` and then subsequently have access to an `express` global. Modules can export whatever they wish, from anything to a rich collection of functions, or even a single primitive.

The example shows how 2 modules of the same name can export totally different things and not interfere with each other.
