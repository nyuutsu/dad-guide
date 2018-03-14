# For Developers

*This section isn't part of the DAD guide! This section is about how to make this website! If you're here to learn about using DAD: you can skip this page and you won't have missed anything.*

## The gist:

* This website is generated using [mdBook](https://github.com/rust-lang/mdBook).

* Website project file is here: [https://github.com/nyuutsu/dad-guide](https://github.com/nyuutsu/dad-guide). Email [Milo](SENDTO:milo.nygren-cassels@ndrn.org) for source access.

* Prerequisites:

  1. install mdBook (that is: download the binary, put it somewhere predictable, then add that location to your $PATH)

  2. clone website source

  3. make changes (if desired)

    * optionally, observe changes in local environment like so:

    ```shell
    mdbook serve --open
    ```

* Build / Deploy process:

  1. run `mdbook build` to generate site in `/book`

  2. copy contents of `book` to server. example:
  
      ```shell
      scp -r /book/* root@nyuu.page:/var/dadbooktest
      ```