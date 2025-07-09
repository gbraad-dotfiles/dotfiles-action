gbraad's Dotfiles `dotfiles` action
===================================

Use dotfiles' `dotfiles`-command to manage the dotfiles deployment

### Usage

```yaml        
      - name: Update to latest dotfiles
        uses: gbraad-dotfiles/dotfiles-action@main
        with:
          action: update
```

> [!NOTE]
> This action does not rely on the installation of the dotfiles. Since it uses the `dot-action`](https://github.com/gbraad-dotfiles/dot-action), it will pull the latest stable version of the dotfiles repository and uses this to manage the deployment of the dotfiles. It is however possible to use the [`install-action`](https://github.com/gbraad-dotfiles/install-action) to ensure the dotfiles are installed before using this action.

Have a look here for an [example workflows](https://github.com/gbraad-dotfiles/actions-test/blob/main/.github/workflows/test-container.yml).