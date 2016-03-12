+++
title = "Quickstart"
+++

Here's a simple example:

```ruby
require 'contracts'

class Example
  include Contracts::Core
  include Contracts::Builtin

  Contract Num => Num
  def double(x)
    x * 2
  end
end

puts Example.new.double("oops")
```

Save this in a file and run it. Notice we are calling `double` with `"oops"`, which is not a number. The contract fails with a detailed error message:

```
ParamContractError: Contract violation for argument 1 of 1:
        Expected: Num,
        Actual: "oops"
        Value guarded in: Example::double
        With Contract: Num => Num
        At: main.rb:8
        ...stack trace...
```

Instead of throwing an exception, you could log it, print a clean error message for your user...whatever you want. contracts.ruby is here to help you handle bugs better, not to get in your way.

