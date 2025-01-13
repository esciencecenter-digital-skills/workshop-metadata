- You need a decent laptop with priviliges to install software. Julia is a compiled language and compiling can be demanding on your CPU. Specifically, something like a Chromebook or similar will definitely not do.
- Install Julia by following the instruction on [the Julia webpage, downloads section](https://julialang.org/downloads/).
- If you have time, explore the [Julia Manual](https://docs.julialang.org/en/v1/). This is not mandatory, but you will learn a lot more in the workshop if you are prepared.
- Prepare the courses package environment. Create directory that you will work in:

```shell
mkdir EfficientJulia
cd EfficientJulia
julia
```

Press `]` to enter package mode:

```shell
(@v1.11) pkg> activate .
(EfficientJulia) pkg> add GLMakie DataFrames BenchmarkTools GeometryBasics IterTools KernelAbstractions Revise Unitful
```

This may take a while (which is why you need to do it in advance).

- Install [VS Code](https://code.visualstudio.com/). VS Code is the de-facto standard IDE for Julia. Within VS Code, install the Julia language plugin.
