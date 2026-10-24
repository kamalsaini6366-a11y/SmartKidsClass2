# Smart Kids – Class 2 (English)

A starter Android app for a Class 2 learner: cartoon-style learning dashboard, English vocabulary and spelling, maths practice, science/EVS, general knowledge, quizzes, stars, saved progress, and spoken prompts.

## Build the APK using GitHub Actions (no Android Studio required)

This ZIP is arranged like the Gym Management project setup that built successfully: the project is inside a folder named `SmartKidsClass2`.

1. Download this ZIP and extract it using WinRAR or Windows' built-in Extract All option.
2. Open your GitHub repository (or create one, e.g. `SmartKidsClass2`).
3. Upload the **entire `SmartKidsClass2` folder** to the repository. Do not upload only the contents of that folder. The repository should show:
   - `SmartKidsClass2`
   - Inside it: `.github`, `app`, `build.gradle`, `settings.gradle`, and other project files.
4. Open the repository's **Code** tab and confirm this file exists at `SmartKidsClass2/.github/workflows/build-apk.yml`.
5. Open **Actions** and refresh the page. Select **Build Smart Kids APK** from the workflow list on the left.
6. Click **Run workflow**, then click the green **Run workflow** button in the dropdown.
7. Open the new workflow run and wait for a green check mark / successful status.
8. In that run, scroll to **Artifacts** and download `SmartKids-Class2-APK`.
9. Extract the downloaded artifact ZIP. It contains `app-debug.apk`.
10. Transfer `app-debug.apk` to your Android phone, tap it to install, and allow installation from that source if Android asks.

### If “Build Smart Kids APK” does not appear
- Check that the workflow file is at exactly `SmartKidsClass2/.github/workflows/build-apk.yml`.
- Make sure the folder and workflow file are committed/pushed to the repository's default branch (usually `main`).
- Refresh **Actions**. If GitHub asks you to enable Actions, enable them for the repository.

## Notes
- This starter uses Android's built-in TextToSpeech voice. An English voice may need to be installed on the phone.
- Lessons and progress are stored locally on the phone; no internet connection is needed after installation for the lesson content.
- This is a debug APK for personal testing, not a Play Store release.
