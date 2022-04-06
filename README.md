## Rust web sample

実践Rustプログラミング入門5章

### init

```
[lowbridgee@04/05 20:14:28] cargo run                                                                     (git)-[main]
    Finished dev [unoptimized + debuginfo] target(s) in 0.05s
     Running `target/debug/todo`

[lowbridgee@04/05 20:15:36] curl localhost:8080
Hello world!%                                                                                                           [lowbridgee@04/05 20:16:11]
```

### テンプレートエンジン

https://docs.rs/askama/latest/askama/

```
cargo add askama
```

結論: deriveマクロよくわからん

### deprecatedとか警告なくそうぜ～

```
all variants have the same postfix: `Error`
`#[warn(clippy::enum_variant_names)]` on by default
remove the postfixes and use full paths to the variants instead of glob imports
for further information visit https://rust-lang.github.io/rust-clippy/master/index.html#enum_variant_names
```

https://rust-lang.github.io/rust-clippy/master/index.html#enum_variant_names

postfix Errorは消したほうがいいとのこと
