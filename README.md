# Create Shipa App Action

This action creates Shipa application

## Inputs

`shipa-action` - path to consolidated Shipa action yml file.

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
        shipa-action: './example/shipa-action.yml'
```
