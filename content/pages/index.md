# contracts.ruby [![Build Status](https://travis-ci.org/egonSchiele/contracts.ruby.png?branch=master)](https://travis-ci.org/egonSchiele/contracts.ruby) [![Join the chat at https://gitter.im/egonSchiele/contracts.ruby](https://img.shields.io/badge/gitter-join%20chat-brightgreen.svg)](https://gitter.im/egonSchiele/contracts.ruby)

Contracts let you clearly – even beautifully – express how your code behaves, and free you from writing tons of boilerplate, defensive code.

## Installation

    gem install contracts

## Simple Example

```ruby
  Contract Num => Num
  def double(x)
```
