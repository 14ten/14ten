```rust
struct Fourteen;

impl Fourteen {
    const ROLE:     &'static str = "Full-stack engineer & sysadmin";
    const LOCATION: &'static str = "Malta";
    const CURRENT:  &'static str = "SafetyNet";
    const CONTACT:  &'static str = "contact@safetynet.at";
    const STACK:    &'static [&'static str] = &[
        "Rust", "TypeScript", "Go", "Lua", "Nix",
    ];
}
```
