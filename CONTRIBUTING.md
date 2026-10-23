# Listing a plugin

To list a plugin here, open a pull request that adds its entry to
`index.json`. A package is listed only after that exact archive is published
and checked, and only if the plugin follows these rules.

1. **Open source.** The plugin's code is published under an open-source
   license: MIT, GPL and its variants, Apache, BSD or similar. A closed-source
   plugin is possible after discussing it with Chilpa's author. For example, a
   streaming company that wants to list its own closed plugin must have public
   Terms of Service and a public Privacy Policy. A plugin built on someone
   else's work credits it, as the
   [Spotify plugin](https://github.com/vicrodh/chilpa-pg-spotify) credits
   Carmine Paolino's Spotifast.

2. **No piracy.** Chilpa is never a piracy tool. A plugin that rips streams or
   downloads music without the right to it is not published in any Chilpa
   repository, this third-party catalog included. Anyone is free to write that
   code and host it in their own repository. Strictly no stream-ripping tools.

3. **Credentials stay with their plugin.** A plugin stores and reads its
   credentials as the SDK's
   [Credentials](https://github.com/vicrodh/chilpa-plugins-sdk/blob/main/wiki/Credentials.md)
   page describes. It never reads, or tries to read, another plugin's
   credentials.

4. **A person writes the pull request.** Build the plugin however you like,
   even if all of it was generated with AI, but the pull request that lists it
   must be written or signed by a person. No emojis and no machine-sounding
   text: the description and the pull request must read easily to a human.

5. **Core changes go to Chilpa.** If a plugin needs a change in Chilpa's core,
   open that pull request in [chilpa](https://github.com/vicrodh/chilpa). The
   change has to be justified as reusable and reliable, so that other plugins
   can use it later.

6. **Reverse engineering is the author's responsibility.** Reverse engineering
   is everyday practice and accepted in most countries. Using it to build a
   plugin is entirely the responsibility of the plugin's author, and using the
   plugin is the responsibility of whoever installs it. That code is not part
   of Chilpa, and neither Chilpa nor its author is responsible for it.

7. **Telemetry is optional and disclosed.** A plugin may
   collect telemetry only with an opt-in or opt-out switch visible in its
   settings. A plugin that collects any says so from installation, in a
   visible place, with its Terms of Service and Privacy Policy. Its README
   explains in plain words what data it collects, where the data goes and how
   it is handled, and includes a liability disclaimer.
