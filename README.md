### I'm Tea.

<a href="https://discord.com/users/s1mply.tea">
  <img src="https://img.shields.io/badge/discord-s1mply.tea-5865F2?style=for-the-badge&logo=discord&logoColor=white" />
</a>
<a href="https://github.com/SimplyTea">
  <img src="https://img.shields.io/badge/github-SimplyTea-181717?style=for-the-badge&logo=github&logoColor=white" />
</a>

```rust
#[derive(Debug)]
pub enum Focus {
    Systems,
    Networking,
    GameModding,
    LowLevelAudio,
    CyberSecurity
}

#[derive(Debug)]
pub struct Tools {
    pub languages: &'static [&'static str],
    pub platforms: &'static [&'static str]
}

#[derive(Debug)]
pub struct Tea {
    pub age: Option<usize>,
    pub pronouns: &'static str,
    pub location: &'static str,
    pub hobbies: &'static [&'static str],
    pub tools: Tools,
    pub status: &'static str,
    pub started_developing: u16,
    pub focus: Focus
}

impl Tea {
    pub fn new() -> Self {
        Self {
            age: Some(19),
            pronouns: "He/Him",
            location: "United States IL",
            hobbies: &["Rust", "Self-Hosting Systens", "Learning new things"],
            tools: Tools { 
                languages: &["Rust", "C", "C++", "C#", "Python", "Shell", "Lua", "Luau", "HTML", "Java", "JavaScript", "CSS", "TypeScript"],
                platforms: &["Windows 10", "Windows 11", "Arch Linux", "Ubuntu"]
            },
            status: "Learning all I can.",
            started_developing: 2019,
            focus: Focus::CyberSecurity
        }
    }

    pub fn favourite_quotes() -> &'static [&'static str] {
        &[
            "If it's hard to explain, it's not done.", 
            "Never tell people how to do things. Tell them what to do and they will surprise you with their ingenuity."
        ]
    }

    pub fn favourite_conversation() -> &'static str {
        "...And has better driver for linux
        What country is that and why do they have better drivers?
        They allow anyone to join.
        So they have open borders?"
    }
}

impl std::fmt::Display for Tea {
    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
        writeln!(f, "Some Cybersecurity nerd.")
    }
}
```
![rust](https://img.shields.io/badge/rust-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)
