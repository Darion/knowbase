# IRC

## Concepts

* `Network` are composed of `servers`. But you connect to network, which decides automatically which server you will use.
* Client
* Nicks are unique in network
* Channel
  * Prefix # - official
  * Prefix ## - unofficial
* Types of input: messages and commands (starts with `/`) 
* User modes
  * ops - `@` prefix
  * voiced - `+` prefix. User who allowed talk in channel

## Connecting to network

```
# irssi:
/connect oftc
/msg NickServ REGISTER password youremail@example.com
/msg NickServ IDENTIFY nick nickserv_password
/join #qtile
```

## Links

* [An IRC quickstart guide](https://opensource.com/article/16/6/irc-quickstart-guide)
* [How do you use IRC?](https://dev.to/nichartley/how-do-you-use-irc-311f)

