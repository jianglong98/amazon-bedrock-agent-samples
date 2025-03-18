# How to Sync Your Fork with the Original Repository

To keep your fork up to date with the original (upstream) repository, follow these steps:

1. **Add the Upstream Repository** (one-time setup)
   ```bash
   git remote add upstream https://github.com/awslabs/amazon-bedrock-agent-samples.git
   ```

2. **Verify Your Remotes**
   ```bash
   git remote -v
   ```
   You should see both `origin` (your fork) and `upstream` (original repository) listed.

3. **Fetch Updates from Upstream**
   ```bash
   git fetch upstream
   ```

4. **Switch to Your Main Branch**
   ```bash
   git checkout main
   ```

5. **Merge Upstream Changes**
   ```bash
   git merge upstream/main
   ```

6. **Push Updates to Your Fork**
   ```bash
   git push origin main
   ```

## Important Notes
- Always make sure your local changes are committed or stashed before syncing
- If you have made changes to files that were also changed in the upstream repository, you might need to resolve merge conflicts
- It's a good practice to sync regularly to keep your fork up to date and minimize merge conflicts