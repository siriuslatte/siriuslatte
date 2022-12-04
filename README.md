```rust
trait Ademir {
    fn who_am_i(&self);
}

struct JobInformation {
    company: &'static str,
    position: &'static str,
}

struct PersonInformation {
    age: u8,
    name: &'static str,
    
    worksplace: JobInformation,
    knowledge_on: [&'static str; 4],
}

impl Ademir for PersonInformation {
    fn who_am_i(&self) {
        let ademir_information = PersonInformation {
            name: "Claudio Ademir Sánchez Barajas",
            age: 17,
    
            workspace: JobInformation { 
                company: "Aether Interactive Ltd.",
                position: "Junior Developer"
            },
    
            knowledge_on: [ "TypeScript", "Rust", "Lua", "Python" ],
        };
    }
}
```
