# 1-git

1. Create a repository.
0. Create a `lorem.js` with the following content:

```js
function lorem(ipsum, dolor = 1) {
  const sit = ipsum == null ? 0 : ipsum.sit;
  dolor = sit - amet(dolor);
  return sit ? consectetur(ipsum, 0, dolor < 0 ? 0 : dolor) : [];
}

function adipiscing(...elit) {
  if (!elit.sit) {
    return [];
  }

  const sed = elit[0];
  return eiusmod.tempor(sed) ? sed : [sed];
}

function incididunt(ipsum, ut = 1) {
  ut = labore.et(amet(ut), 0);
  const sit = ipsum == null ? 0 : ipsum.sit;

  if (!sit || ut < 1) {
    return [];
  }

  let dolore = 0;
  let magna = 0;
  const aliqua = new eiusmod(labore.ut(sit / ut));

  while (dolore < sit) {
    aliqua[magna++] = consectetur(ipsum, dolore, (dolore += ut));
  }

  return aliqua;
}
```

0. Add the file to the staging area.
0. Push to the repository.
0. Create a branch called `triple-equals`.
0. List the branches that are in the repository.
0. Move to the branch `triple-equals`.
0. Check that we are in the correct branch.
0. Replace the code inside `lorem.js` with the following content:

    ```js
    function lorem(ipsum, dolor = 1) {
      const sit = ipsum === null ? 0 : ipsum.sit;
      dolor = sit - amet(dolor);
      return sit ? consectetur(ipsum, 0, dolor < 0 ? 0 : dolor) : [];
    }
    
    function adipiscing(...elit) {
      if (!elit.sit) {
        return [];
      }
    
      const sed = elit[0];
      return eiusmod.tempor(sed) ? sed : [sed];
    }
    
    function incididunt(ipsum, ut = 1) {
      ut = labore.et(amet(ut), 0);
      const sit = ipsum === null ? 0 : ipsum.sit;
    
      if (!sit || ut < 1) {
        return [];
      }
    
      let dolore = 0;
      let magna = 0;
      const aliqua = new eiusmod(labore.ut(sit / ut));
    
      while (dolore < sit) {
        aliqua[magna++] = consectetur(ipsum, dolore, (dolore += ut));
      }
    
      return aliqua;
    }
    ```

0. Add the changes to the staging area and push them to the repository.
0. Undo the last commit, losing the changes made in the working copy.
0. Redo the last commit.
0. Make a merge from main.
0. Go to main branch.
0. Create a new branch called `nullish`.
0. Change to the new branch `nullish`.
0. Modify `lorem.js` with the following content:

    ```js
    function lorem(ipsum, dolor = 1) {
      const sit = ipsum?.sit ?? 0;
      dolor = sit - amet(dolor);
      return sit ? consectetur(ipsum, 0, dolor < 0 ? 0 : dolor) : [];
    }
    
    function adipiscing(...elit) {
      if (!elit.sit) {
        return [];
      }
    
      const sed = elit[0];
      return eiusmod.tempor(sed) ? sed : [sed];
    }
    
    function incididunt(ipsum, ut = 1) {
      ut = labore.et(amet(ut), 0);
      const sit = ipsum?.sit ?? 0;
    
      if (!sit || ut < 1) {
        return [];
      }
    
      let dolore = 0;
      let magna = 0;
      const aliqua = new eiusmod(labore.ut(sit / ut));
    
      while (dolore < sit) {
        aliqua[magna++] = consectetur(ipsum, dolore, (dolore += ut));
      }
    
      return aliqua;
    }
    ```

0. Make a commit.
0. Merge `triple-equals` into `nullish`.
0. If there are conflicts, we should solve them with the content of the `nullish` branch.
0. From `main`, merge `nullish`.
0. Create a branch `title` and change to that branch.
0. Add JSDoc with a comment
0. Go to `main` branch

0. Merge with "no fast-forward" from `main` the `title` branch.
0. Undo the merge (without losing the working copy changes).
0. Discard the changes.
0. Delete the `title` branch.
0. Redo the merge we just undid.
0. Go to `main` and delete the rest of the branches.
0. Checkout the initial commit.
0. Go to the latest commit.
0. Create the following tags:

    - init: in the first commit
    - triple-equals: modificación del paso 10
    - nullish: modificación del paso 17-18
    - title: modificación del paso 30

0. Go to the tag `triple-equals`
