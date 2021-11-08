# Create Shipa App Action

This action creates Shipa application

## Inputs

`app` - path to app.yml file.
`app-env` - path to app-env.yml file.
`network-policy` - path to network-policy.yml file.
`app-deploy` - path to app-deploy.yml file.

## Example usage

```yaml
  steps:
    - name: Checkout
      uses: actions/checkout@v2
    - name: Create shipa app
      uses: rostislavgit/shipa-create-app-action@v0.0.1
      env:
        SHIPA_TOKEN: ${{ secrets.SHIPA_TOKEN }}
        SHIPA_HOST: ${{ secrets.SHIPA_HOST }}
      with:
        app: './example/app.yml'
```
