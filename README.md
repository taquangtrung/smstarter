Spacemacs Starter Kit
-----------------------

# Getting started

- Firstly, clone this repository and rename it to `~/.emacs.d/private`, where
  `.emacs.d` is the directory containing Spacemacs.

- Then, copy the configuration file `.spacemacs` to your home directory

  ```
  cp .spacemacs ~/.spacemacs
  ```

- Add necessary configuration layers into the file `.spacemacs` by modifying the
  lists of configuration layers `dotspacemacs-configuration-layers`
  and packages `dotspacemacs-additional-packages`.

- Finally, run Emacs and choose the suitable editing mode (Emacs or Vim).

# Customize your Emacs

- Add suitable configuration code into the file `smstarter-config.el`.

- Two important configuration functions in `smstarter-config.el` are:
  `smstarter/config-packages` and `smstarter/config-keys`.

- These functions are called from `dotspacemacs/user-config` of `~/.spacemacs`.

# Create a new configuration layer

- To create a new configuration layer:

  ```
  SPC SPC configuration-layer/create-layer RET
  ```

- Then enter the name of your configuration in the prompt.

- A directory named after the created configuration layer will be created here
  along with template files within it (packages.el and extensions.el), more info
  on the meaning of those files can be found in the [documentation](https:/dotspacemacs-additional-packages/github.com/syl20bnr/spacemacs/blob/master/doc/DOCUMENTATION.org#extensions-and-packages).

- Each created file has further guidance written in them.

- Once the configuration is done, restart Emacs to load, install and configure
  your layer.
