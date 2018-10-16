# buck-platform-lazy

Buck should not try to build artefacts that are not required for the current target platform! 

```bash=
buck build :app
```

Buck `2018.08.20.01` works as you would hope! 🎉
