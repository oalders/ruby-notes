# Ruby Notes


<!-- vim-markdown-toc GFM -->

* [exec](#exec)
* [Add Deps](#add-deps)
* [Run Tests](#run-tests)
  * [All Tests](#all-tests)
  * [A Single Test File](#a-single-test-file)
* [Generate Documentation](#generate-documentation)
  * [rdoc](#rdoc)
  * [yard](#yard)
* [Built In Methods](#built-in-methods)
  * [inject()](#inject)
  * [merge()](#merge)
  * [send()](#send)
  * [inspect](#inspect)

<!-- vim-markdown-toc -->

## exec

`bundler exec ruby foo.rb`

## Add Deps

`bundler add hashie`

## Run Tests

### All Tests

`bundler exec rake -t`

### A Single Test File

`bundler exec rspec spec/assessments_spec.rb`

## Generate Documentation

### rdoc

`rdoc`

### yard
```
open http://0.0.0.0:8808 && yard server --reload
```

(Will need to refresh browser once server is up and running).

## Built In Methods

### inject()

Alias for `reduce()`. See
[https://medium.com/@terrancekoar/inject-method-explained-ed531eff9af8](https://medium.com/@terrancekoar/inject-method-explained-ed531eff9af8)

### merge()

A method on a hash. `h1.merge(h2)` merges `h2` into `h1` with the keys of `h2`
(right) taking precedence.

### send()

An instance method of the Object class. The first arg is the name of a method,
followed by the arguments to pass to the method. See
[https://www.programming-books.io/essential/ruby/send-method-79118b73abad44fea7246ea1c03cbc3c](https://www.programming-books.io/essential/ruby/send-method-79118b73abad44fea7246ea1c03cbc3c)

### inspect

An instance method of the Object class for object stringification.

`puts Thing.inspect`
