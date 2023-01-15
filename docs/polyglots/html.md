# HTML-Anything Polyglots
It's fairly easy to make anything into an HTML Polyglot as anything is valid HTML.

Simply insert your HTML into a comment in any language, and most modern browsers will be able to parse it.<br/>
To cover up any visible code, with css, set a container's height & width to cover the whole screen, position to a fixed position at the top-left corner, then set it's background to a solid colouor.

??? note "JS-HTML Example"

    === "JS"

        ```js
        console.log('Hello, World!');
        ```
  
    Turns into

    === "JS"

        ```js
        console.log('Hello, World!'); //<html><head><style>.contentcontainer{position:fixed;top:0;left:0;width:100vw;height:100vh;background:inherit;color:inherit;}</style></head><body><div class="contentcontainer">html here</div></body></html>
        ```

    === "HTML"

        ```html
        console.log('Hello, World!'); //<html><head><style>.contentcontainer{position:fixed;top:0;left:0;width:100vw;height:100vh;background:inherit;color:inherit;}</style></head><body><div class="contentcontainer">html here</div></body></html>
        ```
    
    or
    

    === "JS"

        ```js
        /*<html><head><style>.contentcontainer{position:fixed;top:0;left:0;width:100vw;height:100vh;background:inherit;color:inherit;}</style></head><body><div class="contentcontainer">html here</div></body></html>*/console.log('Hello, World!');
        ```

    === "HTML"

        ```html
        /*<html><head><style>.contentcontainer{position:fixed;top:0;left:0;width:100vw;height:100vh;background:inherit;color:inherit;}</style></head><body><div class="contentcontainer">html here</div></body></html>*/console.log('Hello, World!');
        ```

    ??? abstract "Attribution"
        This example turns [this Lua-JS Polyglot](/polyglots/lua-js#eval-based-vanilla-lua-51js), which is based on [this Luau-JS Polyglot](/polyglots/lua-js#typeof-based-luaujs) by [@jack5079](https://github.com/jack5079), into a Lua-HTML-JS Polyglot.

??? note "Lua-JS-HTML Example"

    === "Lua"

        ```lua
        _=[[/*]]print('lua here');return;--*/]]; console.log(`js here`);
        ```

    === "JS"

        ```js
        _=[[/*]]print('lua here');return;--*/]]; console.log(`js here`);
        ```
  
    Turns into

    === "Lua"

        ```lua
        _=[[/*]]--[=[<html><head><style>.contentcontainer{position:fixed;top:0;left:0;width:100vw;height:100vh;background:inherit;color:inherit;}</style></head><body><div class="contentcontainer">html here</div></body></html>]=]print('lua here');return;--*/]]; eval('console.log(`js here`)');
        ```

    === "JS"

        ```js
        _=[[/*]]--[=[<html><head><style>.contentcontainer{position:fixed;top:0;left:0;width:100vw;height:100vh;background:inherit;color:inherit;}</style></head><body><div class="contentcontainer">html here</div></body></html>]=]print('lua here');return;--*/]]; eval('console.log(`js here`)');
        ```

    === "HTML"

        ```html
        _=[[/*]]--[=[<html><head><style>.contentcontainer{position:fixed;top:0;left:0;width:100vw;height:100vh;background:inherit;color:inherit;}</style></head><body><div class="contentcontainer">html here</div></body></html>]=]print('lua here');return;--*/]]; eval('console.log(`js here`)');
        ```

    or

    === "Lua"

        ```lua
        _=[[/*]]print('lua here');return;--*/]]; eval('console.log(`js here`)');//<html><head><style>.contentcontainer{position:fixed;top:0;left:0;width:100vw;height:100vh;background:inherit;color:inherit;}</style></head><body><div class="contentcontainer">html here</div></body></html>
        ```

    === "JS"

        ```js
        _=[[/*]]print('lua here');return;--*/]]; eval('console.log(`js here`)');//<html><head><style>.contentcontainer{position:fixed;top:0;left:0;width:100vw;height:100vh;background:inherit;color:inherit;}</style></head><body><div class="contentcontainer">html here</div></body></html>
        ```

    === "HTML"

        ```html
        _=[[/*]]print('lua here');return;--*/]]; eval('console.log(`js here`)');//<html><head><style>.contentcontainer{position:fixed;top:0;left:0;width:100vw;height:100vh;background:inherit;color:inherit;}</style></head><body><div class="contentcontainer">html here</div></body></html>
        ```

    ??? abstract "Attribution"
        This example turns [this Lua-JS Polyglot](/polyglots/lua-js#eval-based-vanilla-lua-51js), which is based on [this Luau-JS Polyglot](/polyglots/lua-js#typeof-based-luaujs) by [@jack5079](https://github.com/jack5079), into a Lua-HTML-JS Polyglot.
