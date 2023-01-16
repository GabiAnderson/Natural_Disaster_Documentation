# How to Make a Build





## Build Steps

| Step                                                         | Image                                                        |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| 1. Check out the entire 'Natural Disaster' folder in Perforce | ![](./images/Step1_Checkout.png)                             |
| 2. Copy the 'Natural Disaster' folder to another location, outside of your Perforce workspace | ![](HowToBuild.assets/Step2a_Copy.png)<br />![](./images/Step2b_Paste.png) |
| 3. Revert your change list in Perforce to check everything back in<br /><br />Note: This will take much more time than step 1 | ![](./images/Step3_Revert.png)                               |
| 4. Launch the fresh copy of the project<br /><br />Verify that this is not the real project by checking your source control settings in the bottom right corner - they should be reset/disabled |                                                              |
| 5. Package the project<br /><br />If building for a playtest, a development build is fine. Otherwise, choose shipping build. |                                                              |





## Troubleshooting

If you're encountering errors while trying to package the project, here are some common things that can help:



1. Regenerate Project Files
   - Close the engine
   - Delete the following folders:
     - `Build`
     - `DerivedDataCache`
     - `Intermediate`
     - `Saved`
   - Re-open the engine - the deleted folders should automatically be rebuilt.
   - From here, you can try packaging the project again with the freshly regenerated files.



