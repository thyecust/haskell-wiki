# Newtype

Both `newtype` and `data` are used to create a new type.
The `data` can only be replaced with `newtype` if the type has *=1 constructor* with *=1 field* inside it.

E.g.

```haskell
data Test = Test {
  name :: String,
  value :: Int
}

t = Test { name = "Tianh", value = 21 }

main = putStrLn $ name t
```

`Test` cannot be created using `newtype` becuase it has 1 constructor but 2 fileds.
