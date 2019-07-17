### ffi
---
https://github.com/ffi/ffi

```rb
require 'ffi'

module MyLib
  extend FFI::Library
  ffi_lib 'c'
  attach_function :puts, [ :string ], :int
end

MyLib.puts 'Hello, World using libc!'
```

```sh
gem install ffi
git clone git://github.com/ffi/ffi.git
git submodule update --init --recursive
cd ffi
rake install
```

```
```


