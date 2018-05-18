TYPO3 contribution possibilities
=========

Download Master:
---------------
	1. Open https://wiki.typo3.org/Clone_(Git)
	2. Clone "master" branch
	3. "composer install"
	4. Install TYPO3 --> make sure to have PHP 7.2

Code Review:
---------------
1. Setting up your accounts https://docs.typo3.org/typo3cms/ContributionWorkflowGuide/Account/Index.html
2. Setting up your Git environment https://docs.typo3.org/typo3cms/ContributionWorkflowGuide/Setup/Git/Index.html#setting-up-your-git-environment
3. "Cherry Pick" the patch in Gerrit and "git fetch ...." 
4. Make review and take time to review correctly
5. Reply with "-1" "0" "+1" and perhaps a comment
6. Remember: some core devs can give a "-2" --> with "-2" merging is not possible

Bugfix:
---------------
1. Git clone master branch and install TYPO3
2. Setting up your accounts https://docs.typo3.org/typo3cms/ContributionWorkflowGuide/Account/Index.html
3. Setting up your Git environment https://docs.typo3.org/typo3cms/ContributionWorkflowGuide/Setup/Git/Index.html#setting-up-your-git-environment
4. Make your changes using this guide: https://docs.typo3.org/typo3cms/ContributionWorkflowGuide/BugfixingAZ/Index.html#change-an-existing-patch
5. Commit changes using this guide: https://docs.typo3.org/typo3cms/ContributionWorkflowGuide/Appendix/GeneralTopics/CommitMessage.html
    - IMPORTANT: User correct prefixes like: [TASK] or [BUGFIX]
    - Write first line imperative mood --> [FEATURE] Add option to hide BE search box in list mod
    - Description
    - Relationships: Resolves (must), Related, Releases (must) --> 
        - Resolves / Related = Forge ticket number like: #12345
        - Releases = For which TYPO3 version number is the fix like: master, 8.7, 7.6, 6.2
6. Push patch using this guide: https://docs.typo3.org/typo3cms/ContributionWorkflowGuide/Appendix/GeneralTopics/LifeOfAPatch.html
    - git push origin HEAD:refs/publish/<release-branch> --> git push origin HEAD:refs/publish/master




