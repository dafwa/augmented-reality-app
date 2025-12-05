# Augmented Reality App

An Augmented Reality application built with Unity and the Vuforia Engine.

[Download the APK here.](https://github.com/dafwa/augmented-reality-app/releases/tag/prototype)

---

## ⚠️ IMPORTANT: Do NOT Use "Download ZIP"

**This repository uses Git LFS (Large File Storage) for the Vuforia package.**

If you download this project as a ZIP file from GitHub, the large files will **NOT** be included properly, and the project will be broken. You **must** clone the repository using Git to ensure all assets are downloaded correctly.

---

## Prerequisites

Before cloning this project, ensure you have:

- [**Git**](https://git-scm.com/) installed on your system
- [**Git LFS**](https://git-lfs.github.com/) installed 

To install Git LFS, run:
```bash
git lfs install
```

To verify Git LFS is installed, run:
```bash
git lfs version
```

- **Unity Hub** and a compatible Unity Editor version

---

## Cloning the Repository

Follow these steps exactly to clone the project with all large files:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/dafwa/augmented-reality-app.git
   ```

2. **Navigate into the project directory:**
   ```bash
   cd augmented-reality-app
   ```

3. **Pull all LFS files:**
   ```bash
   git lfs pull
   ```

This ensures all large assets (including the Vuforia package) are downloaded correctly.

---

## Opening the Project in Unity Hub

1. Open **Unity Hub**
2. Click **"Add"** (or **"Open"** depending on your Unity Hub version)
3. Navigate to the cloned `augmented-reality-app` folder
4. Select the folder and click **"Open"** or **"Add"**
5. Unity Hub will detect the project and display it in your projects list
6. Click on the project to open it in the Unity Editor

**Note:** The first time you open the project, Unity may take several minutes to import and compile all assets.

---

## Troubleshooting

### "Library Corrupted" Error

If you see a "Library folder is corrupted" error:

1. Close Unity completely
2. Navigate to the project folder
3. Delete the `Library` folder
4. Reopen the project in Unity Hub

Unity will regenerate the Library folder automatically. This may take a few minutes.

### "Vuforia Missing" or Package Errors

If Vuforia is missing or you see package-related errors:

1. **Verify LFS files were pulled:**
   ```bash
   git lfs ls-files
   ```
   This should show the Vuforia package files.

2. **Re-pull LFS files:**
   ```bash
   git lfs pull
   ```

3. **Check the Packages folder:**
   - Ensure `Packages/` contains the Vuforia package files
   - If files appear to be pointers (very small file sizes), LFS didn't pull correctly

4. **Reinstall Git LFS and re-clone:**
   - If issues persist, reinstall Git LFS
   - Delete the project folder and clone again from scratch

### Assets Not Loading / Gray Materials

If assets appear gray or textures are missing:

1. Verify all LFS files were pulled: `git lfs pull`
2. Reimport all assets: **Assets → Reimport All** in Unity

### Unity Version Mismatch

If Unity warns about a version mismatch:

- Check the `ProjectSettings/ProjectVersion.txt` file for the recommended Unity version
- Install the matching version through Unity Hub if needed
- Or allow Unity to upgrade the project (backup first!)

---

## Additional Resources

- [Unity Documentation](https://docs.unity3d.com/)
- [Vuforia Engine Documentation](https://developer.vuforia.com/)
- [Git LFS Documentation](https://git-lfs.github.com/)

---

## Questions or Issues?

If you encounter problems not covered in this README, please open an issue on the [GitHub repository](https://github.com/dafwa/augmented-reality-app/issues).
