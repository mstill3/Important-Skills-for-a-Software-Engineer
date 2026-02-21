# Useful basic git commands

Version control system (VCS)

## Cloning repository locally

```bash
git clone https://github.com/mstill3/software-engineer-fundamentals
```

## View Changes

### Seeing local changes in repository

```bash
git status
```

### Stage local repository changes

```bash
# for 1 changed file
git add $NEWLY_MODIFIED_FILE

# for entire directory
git add directory/
```

### Commit the changes

```bash
git commit -m "made change"
```

### Push local commit to the remote VCS

```bash
git push
```

### Pulling down remote VCS changes locally

```bash
git pull
```

## Branching

### List branches

```bash
git branch
```

### Create branch

```bash
git checkout -b $NEW_BRANCH_NAME
```

### Checkout branch

```bash
git checkout $BRANCH_NAME
```
