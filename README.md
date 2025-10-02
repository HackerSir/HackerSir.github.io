# HackerSir.github.io
HackerSir WebSite


## Deploy path

### 1. Update [hackersir-web-2022](https://github.com/HackerSir/hackersir-web-2022/tree/master)
After updating hackersir-web-2022, you need to deploy the `gp-pages` with `yarn`.

```bash
yarn install
yarn run build
yarn run install
```

Copy the last commit number (7 digits).

### 2. Deploy Website
Go to this repo. Update submodule
```bash
git submodule update --init --recursive
```

```bash
cd 2022
git fetch --all
```

And then point this page to the gp-pages of hackersir-web-2022.

```bash
git checkout <the last commit number of the gh-pages>
```

```
cd ..
git add 2022
git commit -m "chores: ..."
git push
```
