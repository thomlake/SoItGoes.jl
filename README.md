# SoItGoes.jl
Random useful Julia functions.

## Functions
`chunks{T}(a::Matrix{T}, w::Int, s::Int=1)`
`chunks{T}(a::Vector{T}, w::Int, s::Int=1)`
Split `a` into chunks of size `w` with step `s`. Truncates from end if neccessary.
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