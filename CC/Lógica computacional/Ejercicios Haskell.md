---
fecha : 29-08-2023
---
## Reversa de una lista
``` haskell
reversa :: [a] -> [a]
reversa [] = [] -- caso base
reversa(x:xs) = reversa xs ++ [x] -- recursion
```
## Palíndromo
``` haskell
esPalindromo :: Eq a => [a] -> Bool -- para comparar listas
esPalindromo xs = reversa xs == xs -- comprueba si la reversa es = a la original
```
## Equals
``` haskell
equals :: Eq a => [a] -> [a] -> Bool
equals [] [] = True
equals _ [] = False
equals [] _ = False
equals (x:xs) (y:ys) = x == y && equals xs ys
```
## Naturales
``` haskell
data Nat = Cero | Suc Nat -- Cero: caso base, Suc Nat: función Suc que recibe Nat
```
## Tuplas
``` haskell
data Tupla a b = Tupla a b
```
## Listas
``` haskell
data Lista a = Vacia | Cons a (Lista a) -- Lista a: lista de tipo a
-- ej: Vacia, Cons 1 (Cons 2 Vacia)
```

`Lista a -> [a]`
``` haskell
toHaskell :: Lista a -> [a]
toHaskell Vacia = []
toHaskell (Cons x xs) = x:toHaskell xs
```

`[a] -> Lista a`
``` haskell
fromHaskell :: [a] -> Lista a
fromHaskell [] = Vacia
fromHaskell (x:xs) = Cons x (fromHaskell xs)
```

