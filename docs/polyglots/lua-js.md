# Lua-JS Polyglots
Here's a collection of several Lua-JS Polyglots.

## function-Based Vanilla Lua 5.1/JS

=== "Lua"

    ```lua
    return ([[(()=>{/*js here*/})()/*]] and (function()--[[lua here]];end)())--*/]])[0][0]
    ```

=== "JS"

    ```js
    return ([[(()=>{/*js here*/})()/*]] and (function()--[[lua here]];end)())--*/]])[0][0]
    ```

??? abstract "Attribution"
    This polyglot was created by [@YieldingExploiter](https://github.com/YieldingExploiter)

## Variable-Based Vanilla Lua 5.1/JS

=== "Lua"

    ```lua
    _=[[/*]]print('lua here');return;--*/]]; console.log(`js here`);
    ```

=== "JS"

    ```js
    _=[[/*]]print('lua here');return;--*/]]; console.log(`js here`);
    ```

???+ warning "Warning"
    This polutes the global environment in JS. You can fix this by including `delete globalThis._` in your JS code.<br/>
    Note that doing that will remove any other globals named `_` - This can be hotfixed by replacing `_` with a more "rare" name (say `_polyglot_js_lua_global_ok`)

??? abstract "Attribution"
    This polyglot is based on the [typeof-Based Luau/JS](#typeof-based-luaujs) Polyglot by [@jack5079](https://github.com/jack5079)

## typeof-Based Luau/JS

=== "Lua"

    ```lua
    typeof[[/*]]print'lua here'--*/]];console.log('js here')
    ```

=== "JS"

    ```js
    typeof[[/*]]print'lua here'--*/]];console.log('js here')
    ```

???+ warning "Warning"
    This only works in lua envs with `typeof`, such as Luau.

??? abstract "Attribution"
    This polyglot was created by [@jack5079](https://github.com/jack5079)
