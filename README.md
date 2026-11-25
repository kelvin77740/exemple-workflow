# exemple-workflow

name: Hello World
on:
  - push
  - workflow_dispatch # Permet executar-lo manualment des de la pestanya Actions

jobs:
  say-hello:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout code
        uses: actions/checkout@v4
      - name: Say Hello
        run: echo "Hello, World!"
