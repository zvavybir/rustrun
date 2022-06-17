# rustrun
rustrun is a small program to make [Rust](https://rust-lang.org) into a script language.  Copy `rustrun` to `~/bin/` or `/usr/bin/` and start your script files with `#!/home/your-user-name/bin/rustrun` or `#!/usr/bin/rustrun` respectively.

## Installation
You can choose whether you want to install it locally for your user only or globally for all users.  Doing both is perfectly possible, but unnecessary.

* For your user:
	* Either copy `rustrun` to `~/bin` and add `~/bin` to your `$PATH`,
	* or run `./install_local` (it assumes you use bash or that `~/bin` is already in `$PATH`)
* For all users:
	* Either copy `rustrun` to `/usr/bin`,
	* or run `sudo ./install_global`

## Usage
Start your Rust file with `#!/home/your-user-name/bin/rustrun` or `#!/usr/bin/rustrun` depending on where you installed it to, give the file execution permission (e.g. `chmod +x your-file.rs`) and execute it (e.g. `./your-file.rs`).

## Example
Run `./hello_world.rs` if you want to try rustrun out (it assumes that you installed it globally since there is no way for me to guess your username):
```rust
#!/usr/bin/rustrun

fn main()
{
	println!("Hello, World!");
}
```

## Contributing
Contributions are appreciated, although rustrun doesn't strike me as something that could be meaningfully improved.

## License
rustrun is released under the GNU General Public License version 3 or (at your option) any later version.

For more see [LICENSE.md](https://github.com/zvavybir/rustrun/blob/master/LICENSE.md).