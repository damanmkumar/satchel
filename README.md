## satchel
`satchel` aims to be a thread-safe, persistent, key-value store that can  
be used like regular in-memory associative containers such as `std::map` and  
`std::unordered_map`.

Key-value pairs are read from disk upon opening; modifying operations  
are considered "committed to disk" when they return succesfully. `satchel`  
can be configured at compile-time to either commit these operations  
immediately, or use a write-ahead log to do so lazily.
