<h1 style="text-align:center"><a href="https://github.com/BrunTux/Brun">Brun</a> a 2D tottaly hackable game engine</h1>

How install it

```bash
git clone github.com/BrunTux/Brun
cd Brun
./install.sh # you can link it locally all the engine are just headers files
```

How use it

```cpp
#include <Brun/brun.h>
#include <optional> // you need it for nullopt

int main(void) {
  Brun::Renderer window(600,600,"Hello Brun");

  window.SetBackground("#fff");

  /* the params of window.Run are Load, Update, Draw. 
  The nullopt just means that the func is null and that put the one by default
  */

  window.Run(std::nullopt, std::nullopt, std::nullopt); 
  return 0;
}
```

This code make a white window

For more complete examples go to [examples](https://github.com/BrunTux/Brun/tree/master/examples) folder
