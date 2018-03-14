# [WeeChat](https://hub.docker.com/r/p3lim/weechat/)

Simple Docker image for WeeChat 2.0, allowing you to use it as a always-connected IRC client to remote into, or as a [relay](https://weechat.org/files/doc/stable/weechat_user.en.html#relay_plugin).

### Build Info

- Image: [p3lim/alpine:3.7](https://github.com/p3lim/docker-alpine)
- Ports:
	- `6667` (for normal traffic)
	- `6697` (for encrypted traffic)
	- `9000` (for relaying)
- Volumes:
	- `/config`
- Environment:
	- `PUID` (user id)
	- `PGID` (user group)
	- `TZ` (timezone, e.g. `Europe/Paris`)

### Plugins

WeeChat has plugin support, which this image supports for Lua, Perl, Python and Ruby.  
Plugins are installed the [normal way](https://weechat.org/files/doc/stable/weechat_user.en.html#scripts_plugins).
