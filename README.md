<!-- start title -->

# GitHub Action:Hello World

<!-- end title -->
<!-- start description -->

Greet someone

<!-- end description -->
<!-- start contents -->
<!-- end contents -->
<!-- start usage -->

```yaml
- uses: Unsupervisedcom/action-composite-action-template@undefined
  with:
    # Who to greet
    # Default: World
    who-to-greet: ""
```

<!-- end usage -->
   <!-- start inputs -->

| **Input**          | **Description** | **Default** | **Required** |
| :----------------- | :-------------- | :---------: | :----------: |
| **`who-to-greet`** | Who to greet    |   `World`   |   **true**   |

<!-- end inputs -->
   <!-- start outputs -->

| **Output**      | **Description** | **Default** | **Required** |
| :-------------- | :-------------- | ----------- | ------------ |
| `random-number` | Random number   |             |              |

<!-- end outputs -->
   <!-- start examples -->

### Example usage

```yaml
name: Upload Released Chart
on:
  release:
    types:
      - published
jobs:
  upload-chart-git:
    runs-on: ubuntu-latest
    steps:
      - name: Push Chart
        uses: Unsupervisedcom/action-upload-chart-git@v1
        with:
          token: ${{ secrets.DEPLOYER_CI_TOKEN }}
```

<!-- end examples -->
<!-- start [.github/ghdocs/examples/] -->
<!-- end [.github/ghdocs/examples/] -->
