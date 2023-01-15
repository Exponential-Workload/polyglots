# Is this completely esoteric?

Not completely; however there are only a few normal use-cases for polyglots outside of the esoteric realm.

One such example is, say you want to load some code from a memorable URL (example: `loadstring(game:HttpGetAsync'https://astolfoaim.femboy.cafe')()`) yet also want that url to load in a browser (example: <https://astolfoaim.femboy.cafe>), and don't want to do anything like user-agent checks which may break or be inconsistent.<br/>
In that case, you might decide to use a Lua-[HTML](/polyglots/html) Polyglot.

Another use-case would be, say you have a client API at https://example.com/api & want multiple clients to be able to load it from that URL (say `<script src="https://example.com/api" />` and `loadstring(game:HttpGetAsync('https://example.com/api'))()`), you could use a [Lua-JS](/polyglots/lua-js/) Polyglot.<br/>
Now say you want browsers visiting this URL to not completely break: In that case, you may decide to use a [Lua-JS](/polyglots/lua-js)-[HTML](/polyglots/html) Polyglot.

## Is this mostly esoteric?
Yes. There are very few practical use-cases for Polyglots.
