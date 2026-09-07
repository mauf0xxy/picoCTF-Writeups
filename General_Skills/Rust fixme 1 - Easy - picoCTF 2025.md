# Rust fixme 1 - Easy - picoCTF 2025

```rust
use xor_cryptor::XORCryptor;

fn main() {
    // Key for decryption
    let key = String::from("CSUCKS") // How do we end statements in Rust?

    // Encrypted flag values
    let hex_values = ["41", "30", "20", "63", "4a", "45", "54", "76", "01", "1c", "7e", "59", "63", "e1", "61", "25", "7f", "5a", "60", "50", "11", "38", "1f", "3a", "60", "e9", "62", "20", "0c", "e6", "50", "d3", "35"];

    // Convert the hexadecimal strings to bytes and collect them into a vector
    let encrypted_buffer: Vec<u8> = hex_values.iter()
        .map(|&hex| u8::from_str_radix(hex, 16).unwrap())
        .collect();

    // Create decrpytion object
    let res = XORCryptor::new(&key);
    if res.is_err() {
        ret; // How do we return in rust?
    }
    let xrc = res.unwrap();

    // Decrypt flag and print it out
    let decrypted_buffer = xrc.decrypt_vec(encrypted_buffer);
    println!(
        ":?", // How do we print out a variable in the println function? 
        String::from_utf8_lossy(&decrypted_buffer)
    );
}
```

```verilog
┌──(kali㉿kali)-[~]
└─$ cp -r fixme1 /tmp/rust_proj
                                                                              
┌──(kali㉿kali)-[~]
└─$ cd /tmp/rust_proj
                                                                              
┌──(kali㉿kali)-[/tmp/rust_proj]
└─$ cargo build
    Updating crates.io index
  Downloaded xor_cryptor v1.2.3
  Downloaded either v1.13.0
  Downloaded crossbeam-deque v0.8.5
  Downloaded crossbeam-epoch v0.9.18
  Downloaded crossbeam-utils v0.8.20
  Downloaded rayon-core v1.12.1
  Downloaded rayon v1.10.0
  Downloaded 7 crates (379.2KiB) in 0.50s
   Compiling crossbeam-utils v0.8.20
   Compiling rayon-core v1.12.1
   Compiling either v1.13.0
   Compiling crossbeam-epoch v0.9.18
   Compiling crossbeam-deque v0.8.5
   Compiling rayon v1.10.0
   Compiling xor_cryptor v1.2.3
   Compiling rust_proj v0.1.0 (/tmp/rust_proj)
error: expected `;`, found keyword `let`
 --> src/main.rs:5:37
  |
5 |     let key = String::from("CSUCKS") // How do we end statements in Rust?
  |                                     ^ help: add `;` here
...
8 |     let hex_values = ["41", "30", "20", "63", "4a", "45", "54", "76", "...
  |     --- unexpected token

error: argument never used
  --> src/main.rs:26:9
   |
25 |         ":?", // How do we print out a variable in the println function? 
   |         ---- formatting specifier missing
26 |         String::from_utf8_lossy(&decrypted_buffer)
   |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ argument never used
   |
help: format specifiers use curly braces, consider adding a format specifier
   |
25 |         ":?{}", // How do we print out a variable in the println function? 
   |            ++

error[E0425]: cannot find value `ret` in this scope
  --> src/main.rs:18:9
   |
18 |         ret; // How do we return in rust?
   |         ^^^
   |
help: a local variable with a similar name exists
   |
18 -         ret; // How do we return in rust?
18 +         res; // How do we return in rust?
   |

For more information about this error, try `rustc --explain E0425`.
error: could not compile `rust_proj` (bin "rust_proj") due to 3 previous errors
```

```rust
use xor_cryptor::XORCryptor;

fn main() {
    // Key for decryption
    let key = String::from("CSUCKS"); 

    // Encrypted flag values
    let hex_values = ["41", "30", "20", "63", "4a", "45", "54", "76", "01", "1c", "7e", "59", "63", "e1", "61", "25", "7f", "5a", "60", "50", "11", "38", "1f", "3a", "60", "e9", "62", "20", "0c", "e6", "50", "d3", "35"];

    // Convert the hexadecimal strings to bytes and collect them into a vector
    let encrypted_buffer: Vec<u8> = hex_values.iter()
        .map(|&hex| u8::from_str_radix(hex, 16).unwrap())
        .collect();

    // Create decrpytion object
    let res = XORCryptor::new(&key);
    if res.is_err() {
        return; 
    }
    let xrc = res.unwrap();

    // Decrypt flag and print it out
    let decrypted_buffer = xrc.decrypt_vec(encrypted_buffer);
    println!(
        "{}",  
        String::from_utf8_lossy(&decrypted_buffer)
    );
}
```

```bash
┌──(kali㉿kali)-[/tmp/rust_proj]
└─$ cargo build       
   Compiling rust_proj v0.1.0 (/tmp/rust_proj)
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.13s
                                                                              
┌──(kali㉿kali)-[/tmp/rust_proj]
└─$ cargo run         
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.00s
     Running `target/debug/rust_proj`
```

---

`picoCTF{[REDACTED]}`