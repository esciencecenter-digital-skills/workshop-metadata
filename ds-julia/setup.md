- You need a decent laptop with priviliges to install software. Julia is a compiled language and compiling can be demanding on your CPU. Specifically, something like a Chromebook or similar will definitely not do.
- Install Julia by following the instruction on [the Julia webpage, downloads section](https://julialang.org/downloads/).
- You will learn a lot more in the workshop if you are prepared. Explore the [Julia Manual](https://docs.julialang.org/en/v1/), at least from "Getting Started" until (including) "Scope of Variables". Depending on your experience, this should take upto two hours of your time.
- Prepare the courses package environment. Create directory that you will work in:

```shell
mkdir EfficientJulia
cd EfficientJulia
julia
```

Press `]` to enter package mode:

```shell
(@v1.12) pkg> activate .
(EfficientJulia) pkg> add GLMakie DataFrames BenchmarkTools GeometryBasics IterTools KernelAbstractions Revise Unitful
```

This may take a while (which is why you need to do it in advance).

- Install [VS Code](https://code.visualstudio.com/). VS Code is the de-facto standard IDE for Julia. Within VS Code, install the Julia language plugin.
