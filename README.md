# Grok

Shell enhancing tool for automatic org and repo level command and script aliases.

The main usage of Grok is to set up shareable workflows that automate common org tasks, such as generating API tokens, checking out repos, opening docs, running local servers, ssh-ing into common servers or setting up environment variables.

Grok uses a `.grokrc` file to define various commands. When the `grokrc` command is invoked, the parent directories are traversed to generate a list of available commands, inner directories superseding identical commands. These commands are then aliased to allow the user to invoke the scripts or functions directly. Environment variables can also be set by the `grok` process.

By combining commands with `grok`, one can have commands that navigate between Grok-enabled project, allowing for quick context switching without the `grok` command. The default `grok` distribution includes many useful commands that enable fast checkout of org projects.

Grok allows the org to specify useful commands for managing repos and performing common cross-project tasks, but also allows the projects to maintain their own opinion on "how to grok" them. A "grokline" is a welcome tagline that can be shown to those grokking the repo, inviting them to perform common commands such as "build" or "test", or open more complete help with "help".

It is encouraged to use Grok in creative and perhaps fun ways that might empower your team, such as via slack integrations or with stat tracking. Grok also provides personal overrides that prevent Grok features from the org interfering with developer preference.
