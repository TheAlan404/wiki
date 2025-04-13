# To Rust

## Semicolons

If you dont use a semicolon in a line, it returns the value.
So if you see a line without semicolon in the last line of a function, its actually returning the value.

## Panicking

A panic in rust is basically process.exit(1)

Your code shouldn't panic unless youre ignoring possible errors which is hard in rust

## Option

In Rust, we dont have null. This means optional values must be wrapped in something.

That something is `Option`:

```rs
enum Option<T> {
  Some(T),
  None,
}
```

Now, if this was another language, you think you'd have to check if Option is none or not, do some other stuff to get T right?

No, rust is better. Option has useful functions:

```rs
let x = Some("amy");
let n = None;

x.unwrap() // "amy"
n.unwrap() // panics

x.unwrap_or("may") // "amy"
n.unwrap_or("may") // "may"
```

## Result, Ok, Err

In Rust, there isn't things like `throw Error` or `Exception`
and `try/catch`

Instead, Rust uses `Result`s. Think of it like this:

```rs
fn get_database_value() -> Result<String, DbErr> {}
```

Result is an enum like so:

```rs
enum Result<T, E> {
  Ok(T),
  Err(E),
}
```

## Power

Now yeah these might seem cool, but, rust has these features that make it so nice to use;

### If returning

In JS (or other):

```js
let x = 0;
if (someCondition) {
  otherStuff();
  x = 4;
} else {
  x = 2;
};

// use x here idk
```

Rust:

```rs
let x = if some_condition {
  do_stuff();
  4
} else {
  2
}

//use x here idk
```

Basically if statements can return values.

### If let

You can destructure inside if statements like so;

```rs
if let Ok(value) = some_result {
  // value can be used here
}
```

### Match

Rust's match is like a switch statement sent by gods

```rs
match x {
  "bob" => 5,
  "alice" => 5,
  _ => 0,
}
```

The underscore catches the rest of the possible values.

We can also group values:

```rs
match x {
  "bob" | "alice" => 5,
  _ => 0,
}
```

And also destructure:

```rs
match x {
  Some(name) => get_level(name),
  None => 0,
}
```

And match destructured:

```rs
match x {
  Some("admin") => 100,
  Some(name) => get_level(name),
  None => 0,
}
```

