# copy-bitbucket-access-token-to-clipboard

Simple static (HTML + Javascript) page to be used as Bitbucket OAuth consumer callback URL

# Usage

You can fork this project and host it somewhere else.

## Or, more easily:

Just point your Oath consumer URL callback directly to:

`https://rpagliuca.github.io/copy-bitbucket-access-token-to-clipboard`

*That's it!*

# Detailed Usage

1) Go to Bitbucket Web UI

2) Click on `All workspaces` -> `Select the desired Workspace` -> `Settings` -> `OAuth consumers` -> `Add consumer`

2) Choose a name for your consumer and type into the input `Name`

3) In `Callback URL` type in `https://rpagliuca.github.io/copy-bitbucket-access-token-to-clipboard`

4) Choose the desired `Permissions`

5) Type the optional information as desired (`Description`, `URL`, `Privacy policy URL`, `End user license agreement URL`, etc)

6) Click on the button `Save`

7) After saving, click on the name of newly created consumer and take note of the generated `Key`

8) Print a link from your CLI application to: `https://bitbucket.org/site/oauth2/authorize?response_type=token&client_id=<key_value>`, asking the user to follow the instructions from the webpage. Remember to replace `<key_value>` with the `Key` copied on the previous step.
