# github-pr-list


## Setup

```
$ bundle
```

## Execute

```
$ export GH_TOKEN="YOUR_TOKEN"
$ rake
```

## Output Example


```
(2) org/reponame1
    - 13 : add new feature. : https://github.com/org/reponame1/pull/13
    - 12 : fix typo. : https://github.com/org/reponame1/pull/12
(3) org/reponame2
    - 130 : bump version : https://github.com/org/reponame2/pull/130
    - 129 : add plugin foo : https://github.com/org/reponame2/pull/129
    - 162 : add plugin var : https://github.com/org/reponame2/pull/162
```
