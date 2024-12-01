# CShaderToy

### changes
- RGFW instead of GLFW (portable stb-style GLFW)
- GLAD instead of GLEW (single-header GL loading)
- test + update `autobuild` for windows


### It's that time of the year again, fellas!

<table>
  <tr>
    <td valign="top">
      <img src="https://github.com/alexlnkp/CShaderToy/assets/79400603/44c5f5ea-9e85-4b3a-907f-3912847484f3" alt="infamous-triangle" style="display: block; margin-left: auto; margin-right: auto;" />
    </td>
    <td valign="top">
      <p>Time to learn new stuff, and not just something that is "kinda" cool, but rather something that is <u>EXTREMELY</u> cool!</p>
      <p>For those who thought that programming and art could NOT be combined together, ShaderToy came in to prove You wrong!</p>
      <p>Even though Shader<i>Toy</i> literally has <i>"Toy"</i> in its name, reality is that GLSL shaders are not limited to just being a fun thing to play around with!</p>
      <p>This is when the idea to making this project came to my mind - ShaderToy, but local and on C</p>
    </td>
  </tr>
</table>

GLSL shaders are widely-used by **MOST** game engines, including some of fan favorites, Godot and GameMaker; in other words - learning shaders can come in really handy!

## Getting started
1. To build, do either one of these:
-   Use `./autobuild` shell script for simple building of the project. Zero bloat and build systems, just pure GCC
-   Use GCC itself, don't forget to provide needed flags for APIs that we're using here!
3. ???

```sh
linux : gcc main.c -lX11 -lGL -lXrandr
windows : gcc main.c -lopengl32 -lshell32 -lgdi32 -lwinmm
macos : gcc main.c -framework Foundation -framework AppKit -framework OpenGL -framework CoreVideo
```

Since GLSL shaders can compile at run-time, You don't even have to recompile the main C source file every time you make a small change to the shader!
Just click `R` on your keyboard and all of the shaders will automatically be re-compiled for You! 
This also means that if there's an error in the shader's code, it will be printed out to you verbosely and You will be able to figure out what went wrong!
All of that - on-the-go, no time wasted waiting for the whole program to compile, link, or even restart!

Here's a small demonstration video

[![demo](https://i.ytimg.com/vi/j519qeBmu3Y/maxresdefault.jpg)](https://youtu.be/j519qeBmu3Y "CShaderToy demo")

## Examples
For example shaders, please take a look into [EXAMPLES](EXAMPLES.md)

## Go ahead and make something cool!
