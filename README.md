Sample repository demonstrating how `npm config get cache` depends on the
working directory

Setup:
```
git clone git@github.com:rmacklin/npmrc_cache_config_example.git
cd npmrc_cache_config_example
npm config get cache
cd subdir
npm config get cache
```

Observe the difference in the output:
```
npmrc_cache_config_example/tmp/node_cache
```
vs
```
npmrc_cache_config_example/subdir/tmp/node_cache
```
