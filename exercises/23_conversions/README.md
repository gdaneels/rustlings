# Type conversions

Rust offers a multitude of ways to convert a value of a given type into another type.

The simplest form of type conversion is a type cast expression. It is denoted with the binary operator `as`. For instance, `println!("{}", 1 + 1.0);` would not compile, since `1` is an integer while `1.0` is a float. However, `println!("{}", 1 as f32 + 1.0)` should compile. The exercise [`using_as`](using_as.rs) tries to cover this.

Rust also offers traits that facilitate type conversions upon implementation. These traits can be found under the [`convert`](https://doc.rust-lang.org/std/convert/index.html) module.
The traits are the following:

- `From` and `Into` covered in [`from_into`](from_into.rs)
- `TryFrom` and `TryInto` covered in [`try_from_into`](try_from_into.rs)
- `AsRef` and `AsMut` covered in [`as_ref_mut`](as_ref_mut.rs)

Furthermore, the `std::str` module offers a trait called [`FromStr`](https://doc.rust-lang.org/std/str/trait.FromStr.html) which helps with converting strings into target types via the `parse` method on strings. If properly implemented for a given type `Person`, then `let p: Person = "Mark,20".parse().unwrap()` should both compile and run without panicking.

These should be the main ways ***within the standard library*** to convert data into your desired types.

## Further information

These are not directly covered in the book, but the standard library has a great documentation for it.

- [conversions](https://doc.rust-lang.org/std/convert/index.html)
- [`FromStr` trait](https://doc.rust-lanCustomer 
Order
	
Qty
	
Customer Center
	
Destination 
country
	
Ordered


13958204
	
2
	
ATLAS COPCO BELGIUM NV
	
Belgium
	
16/12/2024


14200834
	
2
	
ATLAS COPCO COMPRESSOR
	
Australia
	
5/02/2025


14200105
	
3
	
ATLAS COPCO KOREA CO LTD
	
South Korea
	
5/02/2025


14274824
	
4
	
ATLAS COPCO SPAIN S.A.E.vision
	
Spain
	
18/02/2025


14338788
	
2
	
ATLAS COPCO (PHILIPPINES) INC.
	
Philippines
	
28/02/2025


14340751
	
2
	
ATLAS COPCO SCHWEIZ AG
	
Switzerland
	
28/02/2025


14336760
	
1
	
ATLAS COPCO MEXICANA SA DE CV
	
Mexico
	
27/feb


14182663
	
3
	
AC COMPRESSORS LLC
	
United States
	
31/01/2025


14305622
	
6
	
ATLAS COPCO MOROCCO
	
Morocco
	
24/02/2025


14000362
	
3
	
ATLAS COPCO MOROCCO
	
Morocco
	
25/12/2024g.org/std/str/trait.FromStr.html)
