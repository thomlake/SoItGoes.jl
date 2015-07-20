# SoItGoes.jl
Random useful Julia functions.

## Functions
##### `chunks(a, w, s=1)`

Split a Vector or Matrix `a` into chunks of size `w` with step `s`. Truncates from end if neccessary.
```
julia> chunk(collect(1:20), 5, 3)
6-element Array{Array{Int64,1},1}:
 [1,2,3,4,5]     
 [4,5,6,7,8]     
 [7,8,9,10,11]   
 [10,11,12,13,14]
 [13,14,15,16,17]
 [16,17,18,19,20]
```

`flatten(a::Array)`

Flatten an array without a copy, borrowed from [this](https://groups.google.com/d/msg/julia-users/1QrIhbRA8hs/9PcNeO2N9wQJ) julia-users thread.


`tally{I<:Integer}(a::Array{I})`

Return a vector `r` such that `r[i]` = # of occurences of `i` in `a`.

`countmax{I<:Integer}(a::Array{I})`

Return the most frequently occuring integer in `a`.


