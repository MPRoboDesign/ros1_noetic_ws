# DEV - INSTRUCTION

## Instruction for adding new package
Let's say that a ros package name PKG is required,
- Browse and find the <git_url> for the source code of PKG.
- Find the respective <branch_name>.
- Navigate to src of the workspace by running:
```
cd src
```
- Run the following to add the package:
```
git submodule add --branch <branch_name> <git_url> <pkg_name>
```
- Navigate back to workspace by running:
```
cd ..
```
- Add it to git by running:
```
git add .
```
- Commit it along with a commit message:
```
git commit -m "<message>"
```
- Push it to Git hub by running:
```
git push
```

## Instruction for push into specific branch
- Run the following:
```
git push -u origin <branch>
```

## Instruction to properly delete a package
Let's say we want to remove a package named PKG.
- Navigate to src, by running:
```
cd src
```
- Remove the package by running:
```
rm -r PKG
```
- Navigate back to workspace by running:
```
cd ..
```
- First update the submodules list by running:
```
git submodule update
```
- Now add the changes to the git by running:
```
git add .
```
- Commit it along with a commit message:
```
git commit -m "<message>"
```
- Push it to Git hub by running:
```
git push
```
