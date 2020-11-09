# 2020-election-fraud

1. download pa voting data and unzip into ./data/pa
2. make sure mysql is install and have root user without password (for local ONLY!)
3. run `./load-data`

```shell
git clone git@github.com:blai/2020-election-fraud.git
cd 2020-election-frand
# if need to reload data
# ./reset-data
./load-data
```

#### WARNING

For query performance, many indexies were added, check `load-data` for detail. This will make importing data slow, if you prefer to trade faster data import for slower queries, remove the index in `load-data` script.

#### Expected `data` folder
```
# ❯ tree data -L 1

data
└── pa

```
