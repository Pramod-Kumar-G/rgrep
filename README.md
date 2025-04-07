# rgrep

A lightweight, fast, and minimalistic command-line search tool written in Rust, inspired by `grep`.


## 📦 Features

- 🔍 Search for lines that contain a given string
- 🆎 Case-insensitive search via environment variable
- ⚡ Fast and lightweight
- 🦀 Built with Rust — safe and performant

## 🚀 Usage

```bash
rgrep <query> <file_path>
```

## 📄 Example

```bash
rgrep to poem.txt
```
This will print all lines from poem.txt that contain the word "to".

## 🔡 Case-insensitive search

You can enable case-insensitive search by setting the IGNORE_CASE environment variable:
```bash
IGNORE_CASE=true rgrep to poem.txt
```
This will match "to", "To", "TO", "tO".

## 🛠 Installation
1. Clone the repo
```bash
git clone https://github.com/yourusername/rgrep.git
cd rgrep
```
2. Build the project in release mode
```bash
cargo build --release
```
3. Move the binary to a directory in your $PATH
```bash
cp target/release/rgrep ~/.local/bin/
```
  If ~/.local/bin is not in your path, add this to your shell config (e.g., ~/.zshrc, ~/.bashrc):
```bash
export PATH="$HOME/.local/bin:$PATH"
```
Then reload your shell:
```bash
source ~/.zshrc  # or source ~/.bashrc
```
4. Run it globally
```bash
rgrep hello notes.txt
```

## 👨‍💻 Why I Built This

This project was built to learn Rust by recreating a lightweight version of grep. It covers:

   - File I/O

   - Environment variables

   - Building real CLI tools in Rust

## 📜 Note

This was just a small learning project built while going through *The Rust Programming Language* book.  
Feel free to use, modify, or share it — no license needed.
