## Conda Commands

Create new environment

```
conda create --name <name> <package=version>
```

Activate and use env

```
conda activate <env-name>
```

List environments

```
conda env list
```

List packages

```
conda list
```

Install packages (last version available)

```
conda install <package-name>
```

Install packages (specific version)

```
conda install <package-name=version>
```

See package version installed

```
conda list <package-name>
```

Remove packages

```
conda remove <package-name>
```

Remove env

```
conda env remove --name <env-name>
```

Install package from specific channel

```
conda install --channel <channel-name> <package-name>
```

See env revisions

```
conda list --revision
```

Return to a previous revision

```
conda install --revision <revision-number>
```

Export env

```
conda env export
```

Export env with only packages versions

```
conda env export --no-builds
```

Export env with specified packages from user (Best way)

```
conda env export --from-history
```

Export env with specified packages from user using file (Best way)

```
conda env export --from-history --file <filename.yml>
```

Import env from file

```
conda env create --file <filename.yml>
```
