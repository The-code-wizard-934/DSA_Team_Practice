# 🤝 CONTRIBUTING.md – Guidelines for DSA Team Practice Repo (Branch-Based Workflow)

This file explains **how to contribute correctly** to the repository using branches and PRs so that the repository stays clean, organized, and conflict-free.

---

## 1️⃣ Work in Your Own Folder Only

Every member must work only inside their personal folder:

```
Members/<YourName>/Questions/
Members/<YourName>/Solutions/
Members/<YourName>/Progress.md
```

❌ Do NOT edit other member’s folders.

---

## 2️⃣ Adding New Questions

1. Open your Questions folder: `Members/<YourName>/Questions/`
2. Open or create a `.md` file for the topic, e.g., `Arrays.md`
3. Add questions in this format:

```markdown
1. Two Sum – https://leetcode.com/problems/two-sum/
2. Maximum Subarray – https://leetcode.com/problems/maximum-subarray/
```

4. Save the file

---

## 3️⃣ Writing Solutions

1. Open your Solutions folder: `Members/<YourName>/Solutions/<Topic>/`
2. Create **one file per problem**, e.g.: `two_sum.cpp`
3. Use this header format inside each solution file:

```cpp
/*
Problem: Two Sum
Platform: LeetCode
Difficulty: Easy
Approach: Hashmap
Time Complexity: O(n)
Space Complexity: O(n)
*/
```

4. Write your solution below the header

### Naming Conventions

* Use lowercase letters and underscores: `two_sum.cpp`
* One problem per file
* Include topic folder: `Solutions/Arrays/two_sum.cpp`

---

## 4️⃣ Updating Progress

Track daily progress in `Progress.md` inside your folder:

```markdown
| Date | Problem | Topic | Status | Language |
|------|---------|-------|--------|----------|
| 2026-01-16 | Two Sum | Arrays | Done | C++ |
```

---

## 5️⃣ Branch Workflow

### Step 1 – Pull Latest Main

Always start with:

```bash
git checkout main
git pull origin main
```

### Step 2 – Create Your Branch

```bash
git checkout -b <yourname-topic>
```

Example: `yash-arrays`

### Step 3 – Add Files and Commit

```bash
git add .
git commit -m "add: two sum solution by <yourname>"
```

### Step 4 – Push Branch

```bash
git push origin <yourname-topic>
```

---

## 6️⃣ Pull Request (PR) Workflow

1. Open GitHub → Repository → Pull Requests → New Pull Request
2. Select your branch → base: main
3. Add description: problem name, topic, difficulty, approach
4. Submit PR
5. Team reviews → Merge into main

> PR ensures main branch stays clean, reviewed, and conflict-free.

---

## 7️⃣ Rules Summary

* Work ONLY in your folder
* One problem = one file
* Use proper naming conventions
* Include complexity and approach in every solution
* Pull main before creating branch
* Commit regularly with clear messages
* Update progress daily
* Use branches + PR for all contributions

---

## 8️⃣ Error Handling Tips

* Push rejected → `git pull origin main` then `git push origin <branch>`
* Undo changes → `git restore .`
* Remove last commit → `git reset --soft HEAD~1`
* Merge conflict → resolve manually, then:

```bash
git add .
git commit -m "resolve conflict"
git push origin <branch>
```

Follow these steps to contribute safely, collaboratively, and professionally while learning DSA effectively. 🚀
